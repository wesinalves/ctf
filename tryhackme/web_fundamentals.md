# Web Fundamentals room from tryhackme.com

# What was done

This room is designed as a basic intro to how the web works.

We'll cover HTTP requests and responses, web servers, cookies and then put them all to use in a mini Capture the Flag at the end.

# What was learnt

* finding the server (DNS request)
* loading content
    * request verbs (GET, POST)
    * common port (80)
    * content of web page (HTML, CSS, Javascript)
* Responses
    * 100-199: Information
    * 200-299: Successes (200 OK is the "normal" response for a GET)
    * 300-399: Redirects (the information you want is elsewhere)
    * 400-499: Client errors (You did something wrong, like asking for something that doesn't exist)
    * 500-599: Server errors (The server tried, but something went wrong on their side)
* Cookies

Cookies are small bits of data that are stored in your browser. Each browser will store them separately, so cookies in Chrome won't be available in Firefox. They have a huge number of uses, but the most common are either session management or advertising (tracking cookies). Cookies are normally sent with every HTTP request made to a server.

* Curl

curl *url* (default get verb)
curl -X POST *url* --data *data* (send a post request)
curl -d *data* -X POST *url* (send a post request)
curl -c - *url* (retrieve a cookie)
curl -v --cookie *key=value* *url* (send a cookie)

# tools

curl 

tab storage on devtools