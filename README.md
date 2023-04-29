# image-lambda
Code Fellows - 401 - Lab 17

## How To Use
This lambda function will be triggered any time a user uploads a new file/image to the target S3 bucket.

If you want to use it for yourself on your own bucket, just copy/paste the code in `index.mjs` into your own lambda function and set it to trigger on your own S3 bucket.

## Issues Encountered
I was beating my head against the wall for an unnecessary amount of time because `manifest.Body` and `manifest.Body.toString()` were not returning the data that I was expecting so therefore I could not parse the JSON data back into a usable array that I could add new values into. After like 30-40 minutes of digging around online for answers I finally had to watch the lecture video from class 18 and thankfully Jacob walked through the exact issue I was having and all I had to do was use `transformToString()` instead of `toString()`.

## JSON

https://401-lab17.s3.us-west-2.amazonaws.com/images.json
