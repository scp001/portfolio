#About

This is simple FAQ document that covers most frequent use cases of the website and blog

---

##Website

In order to edit content of the website:

1. Download "website" folder.
2. Open it at your PC and open `index.html` file
3. Make changes
4. Upload updated `index.html` file to the Amazon Web Services S3 bucket with name `yadixing.ca`

---

##Blog

###In case blog is not loading:

1. Login to your AWS account
2. Go to `Services > EC2`
3. Go to `Running Instances`
4. Choose instance, press `Actions`, then  `Instance State > Reboot`
5. Wait 1-2 minutes for system to restart and visit web page

###To delete post:

1. Got to http://blog.yadixing.ca/admin
2. Login using your credentials
3. Choose post
4. Start editing it
5. Press **"Unpublish"**, now post won`t appear at the blog front page any more.
6. Press black cross to the left of `Unpublish` button to delete it completely

###To add video (e.g. from YouTube):

1. Go to video.
2. Right-click at video frame, choose "Copy emded code" and paste to blog post. Should look like:
```
<iframe width="1280" height="720" src="https://www.youtube.com/embed/QtXby3twMmI" 
frameborder="0" allowfullscreen></iframe>
```

Change its width and height if you want.

###To add image, style post:

Use inline html and css. E.g.

`<img src="someurl.com"/>`

`<a href="linktoanywhere.com">Link to anywhere</>` etc.

###To run blog at your local machine (you need to have `nodejs` and `npm` installed):

1. Download "blog" folder.
2. Open terminal and enter "blog" folder at you PC.
3. Run `npm install hexo-cli -g`
4. Run `npm install`
5. Run `hexo server -d`
6. Open "localhost:8080" in your browser

---

If you have any more questions feel free to contact me.

Good luck!
