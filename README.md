# mp3lrc
A small collection of mp3 songs with their LRC file

## API Documentation

This is a lightweight web service, (REST interface), which provides an easy way to access **`mp3lrc`** data.
The API works through simple commands, so there should not be a problem coding some nice applications.
This API contains total **1** route(s)


## API Endpoints

All the API endpoints return the same data structure as below

|Returned Key|Description|Example|
|------------|-----------|-------|
|error|The returned status for the API call, can be either 'true' or 'false'|true|
|message|Either the error message or the successful message|OK|
|data|If 'error' is returned as 'false' the API query results will be inside 'data'|data|


**Success Response Format**

```json
{
    "error": false,
    "message": "SUCCESS_MESSAGE",
    "data": {}
}
```

**Error Response Format**

```json
{
    "error": true,
    "message": "ERROR_MESSAGE"
}
```

## Routes



#### 1 . /get_songs

- Method : **GET**
- URL : [/get_songs](http://theapache64.com/mock_api/get_json/mp3lrc/get_songs)
- MockURL : [get_songs](http://theapache64.com/mock_api/get_json/mp3lrc/get_songs?is_skip_auth=true)



**Response Body**
```json
{
  "error" : false,
  "message" : "OK",
  "data" : {
    "songs" : [ {
      "mp3_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/carly%20rae%20jepsen%20-%20call%20me%20maybe.mp3",
      "lrc_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/carly%20rae%20jepsen%20-%20call%20me%20maybe.lrc",
      "artist" : "Carly Rae Jepsen",
      "title" : "Call Me Maybe",
      "base_file_name" : "carly rae jepsen - call me maybe"
    }, {
      "mp3_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/michael%20bolton%20-%20when%20a%20man%20loves%20a%20woman.mp3",
      "lrc_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/michael%20bolton%20-%20when%20a%20man%20loves%20a%20woman.lrc",
      "artist" : "MIchael Bolton",
      "title" : "When A Man Loves A Woman",
      "base_file_name" : "michael bolton - when a man loves a woman"
    }, {
      "mp3_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/egil%20olsen%20-%20sleep%20with%20you.mp3",
      "lrc_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/egil%20olsen%20-%20sleep%20with%20you.lrc",
      "artist" : "Egil Olsen",
      "title" : "Sleep With You",
      "base_file_name" : "egil olsen - sleep with you"
    }, {
      "mp3_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/anastacia%20-%20defeated.mp3",
      "lrc_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/anastacia%20-%20defeated.lrc",
      "artist" : "Anastacia",
      "title" : "Defeated",
      "base_file_name" : "anastacia - defeated"
    }, {
      "mp3_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/ke%24ha%20-%20tik%20tok.mp3",
      "lrc_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/ke%24ha%20-%20tik%20tok.lrc",
      "artist" : "Ke$ha",
      "title" : "Tik Tok",
      "base_file_name" : "ke$ha - tik tok"
    }, {
      "mp3_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/the%20pussycat%20dolls%20-%20buttons.mp3",
      "lrc_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/the%20pussycat%20dolls%20-%20buttons.lrc",
      "artist" : "The Pussycat Dolls",
      "title" : "Buttons",
      "base_file_name" : "the pussycat dolls - buttons"
    }, {
      "mp3_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/lenka%20-%20the%20show.mp3",
      "lrc_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/lenka%20-%20the%20show.lrc",
      "artist" : "Lenka",
      "title" : "The Show",
      "base_file_name" : "lenka - the show"
    }, {
      "mp3_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/taylor%20swift%20-%20love%20story.mp3",
      "lrc_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/taylor%20swift%20-%20love%20story.lrc",
      "artist" : "Taylor Swift",
      "title" : "Love Story",
      "base_file_name" : "taylor swift - love story"
    }, {
      "mp3_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/maroon%205%20-%20moves%20like%20jagger.mp3",
      "lrc_url" : "https://raw.githubusercontent.com/theapache64/mp3lrc/master/maroon%205%20-%20moves%20like%20jagger.lrc",
      "artist" : "Maroon 5",
      "title" : "Moves Like Jagger",
      "base_file_name" : "maroon 5 - moves like jagger"
    } ]
  }
}
```



