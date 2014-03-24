####custom-google-loader

This is a custom version of google loader that I'm using for GpsTracker. Google's version of the loader which is here:

https://developers.google.com/loader/

does not seem to be supported anymore (jquery is at version 1.7.1 which is a few years old). So what I've done is removed all of the other frameworks that I'm not using (such as mooworks, scriptaculous, etc.) and updated it to support jquery version 1.11.0 and 2.1.0. I also changed the google urls to https. This version is stripped down and supports jquery and google maps.

I've minified the code using Google's closure minifier set on "simple".

http://closure-compiler.appspot.com/home

To use it, just install it on your website and add the script like this:

<script src="custom-google-loader-1.0.0.min.js"></script>
and call it like this:

google.load('jquery', '1.11.0');
or this for maps:

google.load("maps", "3", {
    other_params: "sensor=false&libraries=adsense"
});






