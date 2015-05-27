This is a snapin using javascript and the Infoblox WAPI to implement an efficient set of rapid search forms.

To use this, enable File Distribution on the Grid Master and upload and unzip into the root folder of File Distribution on the Grid Master.  It will create the following folder structure so make sure it doesn't overwrite anything in ./snapins/search/...:

.
./snapins
./snapins/search
./snapins/search/...files...

Open a broswer and go to http://[server]/snapins/search


*HTTP Redirection Error

If you are using HTTP to HTTPS redirect and the UI complains when you turn on
HTTP File Distribution, you can disable redirect and place this in the root directory of File Distribution in a file named index.html.  It will cause the redirection from HTTP to HTTPS:

<head>
<meta HTTP-EQUIV="REFRESH" content="0; url=https://[your infoblox gridmaster ip or dns]">
</head>
