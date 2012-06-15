North-American-Octo-Hipster
===========================

_I loved the stupid suggestion title that GitHub gave me so much that I just had to use it_

Uses NodeJS to make a command line server that can serve static files only. Includes a bundled copy of Node.exe which is portable Node for windows. The entire application runs out of the server.js file and weighs in at only 1kb of code and under 5mb with the included node executable.

To use either drag the server.js files onto node.exe or from the command line run using `node server.js`

The default port that the server runs on is `8888`. To change this, edit the `server.js` file in your favourite text editor and on line 5 change 
`port = process.argv[2] || 8888;` to be `port = process.argv[2] || 80;` if you wanted it running on port 80 for instance!

The application looks at the URL to determine the resource it is trying to get at. If the URL is a directory i.e. the root of the url `/` it will attempt to find an index.htm file to serve as the content.

It will produce 404 errors on an inability to find a resource requested. Will also produce 500 errors if it fails to read a file because it is corrupt for instance.

Uses the [SimpleTape](http://creattica.com/free-css-templates/simpletape-free-minimalistic-site-template/79129) free html template theme as a demo.

I use this on the go to demonstrate simple web pages to people, as I can turn any machine into a web server with simply a few clicks now.