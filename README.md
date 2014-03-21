Op3nVoice curl examples
==============

This project is just a holder for examples of using the Op3nVoice API using curl.

## Create an audio record:

curl --data "media_url={audio file}" https://api-beta.op3nvoice.com/v1/audio --header "Authorization: Bearer {auth key}" | python -mjson.tool

## Retrieve a specific record:

curl https://api-beta.op3nvoice.com/v1/audio/{bundle id} --header "Authorization: Bearer {auth key}" | python -mjson.tool

## List all records:

curl https://api-beta.op3nvoice.com/v1/audio --header "Authorization: Bearer {auth key}" | python -mjson.tool

## Search:

curl https://api-beta.op3nvoice.com/v1/search?query={search term} --header "Authorization: Bearer {auth key}" | python -mjson.tool