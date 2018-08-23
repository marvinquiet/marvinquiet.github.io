### Quick Web Development

I am fresh new to Web Development, which means, I haven't developed any application related to web before. However, due to research reason, we could not always let researchers download our Python or R package, and run data themselves. For one, our simulation consumes a lot of CPU cores which not every researcher owns; for another, there are plenty installation issues due to different OS. Fortunately, I have experience in programming, especially in Python and Java. Then, why not having a try? 

### Step 1: Choose a Framework

Web development mostly could be divided into front-end, back-end and full-stack. Thanks to those **GREAT** Open Source contributors, there are lots of frameworks to choose from, such as [Django](https://www.djangoproject.com/), [Flask](http://flask.pocoo.org/), [RoR](https://rubyonrails.org/). Each has its advantages and disadvantages. Since my project would be quite tiny, I chose Flask as my Web Framework. 

From my perspective, Flask would be more tiny and lightweight. For a beginner, if you don't want to waste too much time on learning how a framework works, then I think Flask would be a good choice. 

### Step2: Learn Basic Knowledge

Take Flask as an example, the only thing you need to know is:

* How to run an app

  ```python
  # hello.py
  from flask import Flask
  app = Flask(__name__)
  
  @app.route("/")
  def hello():
      return "Hello World!"
  ```

  ```shell
  $ FLASK_APP=hello.py flask run
  # "Hello World!" gonna show on localhost:5000
  ```

* How flask routes

  ```python
  @app.route('/') # localhost:5000/
  def index():
      return 'Index Page'  
  
  @app.route('/hello') # localhost:5000/hello
  def hello():
      return 'Hello, World'
  ```

* How flask uses variables through URL

  ```python
  @app.route('/user/<username>') # localhost:5000/user/<username>
  def show_user_profile(username):
      # show the user profile for that user
      return 'User %s' % username
  ```

  **Note**: URL is used for the website, not equivalent to a file path. If you need URL variables to generate a file path, do it inside the function by using the parameters passed by the URL.

  Here is a small example on passing URL to download file. I am not sure if there is a better way, but it works.

  ```python
  from flask import send_from_directory
  
  # URL: /download/123___a.txt
  @app.route('/download/<userkey_filename>')
  def download_file(userkey_filename):
      user_key, filename = userkey_filename.split('___')  # user_key: 123, filename: a.txt
      download_path = os.path.join(user_key, 'download')
      return send_from_directory(download_path, filename)
  ```

  In this case, it does not matter what name is your function, since I do not call it from other part. What I do is to bind the URL with the file path. Then when I pass the result containing both of them to the html, when the URL is clicked, it will directly goes to my file path, and download the file.

  ```python
  from flask import render_template
  
  @app.route('/result', methods=['GET', 'POST'])
  def show_result():
      results = {'url_file': ['/download/123___a.txt', 'a.txt']}
      return render_template('result.html', results=results) # passing values to html
  ```

  ```html
  {% for urlFile in results['url_file'] %}
     <a href="{{ urlFile[0] }}" download> {{ urlFile[1] }}</a>
  {% endfor %}
  ```

  Therefore, in thise case, `href = {{ urlFile[0] }}` related to the url, and `{{ urlFile[1] }}` will show file name.

  When the link is clicked, it will trigger the `@app.route('/download/<userkey_filename>')` to find the file directory, and sent the file from that directory.

* How the project package looks like

  A project should looks alike [flask layout](http://flask.pocoo.org/docs/1.0/tutorial/layout/), however, since I use file instead of database and I do not focus on those fancy demonstrations, I compress it into this:

  ```shell
  /home/user/Projects/flask-tutorial			
  ├── __init__.py
  ├── frontend.py         # only do things related to frontend
  ├── do_*.py             # do things related to backend logic
  ├── templates/          # html
  │   ├── base.html
  │   └── error.html
  ├──static/              # static files
  │   └── style.css
  ├── db.json             # file storage
  ├── venv/
  ├── setup.py
  └── MANIFEST.in
  ```

### Step3: Use Open Source Templates

[Bootstrap](https://getbootstrap.com/) is a GREAT template for those who don't want to spend much time on how to adjust demonstration. You even don't need to download the package, just use [BoostrapCDN](https://www.bootstrapcdn.com/) and it will access the network resource to retrieve the style. 

Pick one of the [Boostrap examples](https://getbootstrap.com/docs/4.1/examples/), right click View Page Source. Select all, copy, paste it into one of your templates. 

Change the local resource

```html
<!-- Bootstrap core CSS -->
<link href="../../dist/css/bootstrap.min.css" rel="stylesheet">
```

into CDN resource:  

```html
<!-- Bootstrap core CSS -->
<link href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.2/css/bootstrap.min.css" rel="stylesheet">
```

### Step4: Start Building Your Own

This is a passage which not only a tutorial, but also a reminder. Skills could be forgot easily without use. I hope when I finish my current project on [Find the Transcriptional Binding](https://github.com/marvinquiet/flask-tf-binding) expectedly before October due to server reasons, I will publish a full link here. Let's just get it!



**Special thanks to [Jiaying Lu](https://lujiaying.github.io/)** who taught me these quick web development skills and gave me technical instructions with no reservation. 