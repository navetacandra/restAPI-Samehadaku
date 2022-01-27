## Samehadaku restAPI

This rest api is unofficial. So I am not responsible if there is incomplete/broken data.

**All data taken from**: [Samehadaku](https://194.163.183.129)

### TODO

- [x] Home (Anime This Season)
- [x] Ongoing
  - [x] Pagination
- [x] Schedule
- [x] Genre List
  - [x] Anime By Genre With Pagination
- [x] Detail Anime
  - [x] Detail
  - [x] Batch
  - [x] Episode List
- [x] Detail Batch
  - [x] Detail
  - [x] Download Link
- [x] Detail Episode
  - [x] Pagination Per Episode
  - [x] Streaming Link
  - [x] Download Link
- [x] Search
- [ ] Refactor Code Anime & Batch Detail Functions (_If It's Possible. Lieur soal na_)

### Usage

1. Clone this repository

```bash
mkdir -p ~/Documents/git && git clone --depth=1 https://github.com/Hanivan/restAPI-Samehadaku.git ~/Documents/git/restAPI-Samehadaku && cd ~/Documents/git/restAPI-Samehadaku
```

2. Install packages (use `yarn` or `npm`)

```bash
yarn install
```

3. Start server

```bash
yarn start
```

or

```
yarn dev (for development)
```

### API Documentation

**API Path**: [https://samehadaku-api.herokuapp.com/api](https://samehadaku-api.herokuapp.com/api)<br>
**API Version**: v1

| Endpoint                   | Params        | Description                        |
| -------------------------- | ------------- | ---------------------------------- |
| /home                      | -             | Homepage (Current Season)          |
| /anime                     | -             | List All Anime                     |
| /anime/page/${page}        | pageNumber    | Anime Pagination                   |
| /anime/${id}               | id            | Detail Anime                       |
| /ongoing                   | -             | List All Ongoing Anime             |
| /ongoing/page/${page}      | pageNumber    | Ongoing Pagination                 |
| /movie                     | -             | List All Anime Movie               |
| /movie/page/${page}        | pageNumber    | Anime Movie Pagination             |
| /genres                    | -             | List All Genre                     |
| /genres/${id}              | id            | Show Anime by Genre                |
| /genres/${id}/page/${page} | id,pageNumber | ~~ Anime by Genre With Pagination  |
| /batch                     | -             | List All Anime Batch               |
| /batch/page/${page}        | pageNumber    | Batch Pagination                   |
| /batch/${id}               | id            | Detail Anime Batch                 |
| /eps/${id}                 | id            | ~~ Anime Episode                   |
| /schedule                  | -             | Schedule Anime                     |
| /studio/${id}              | id            | Show Anime by Studio               |
| /studio/${id}/page/${page} | id,pageNumber | ~~ Anime by Studio With Pagination |
| /season/${id}              | id            | ~~ Anime by Season                 |
| /season/${id}/page/${page} | id,pageNumber | ~~ Anime by Season With Pagination |
| /search/${query}           | query         | Search Anime                       |

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Development Details

**Start Work**: Sunday, 16 January 2022; 16:-- PM WIB<br>
**Finished Work**: Thursday, 27 January 2022; 15:-- PM WIB

**Absence**: Monday, 24 January 2022<br>
**Reason**: Learn GoLang

Thank you [ Kaede-No-Ki/otakudesu-rest-api](https://github.com/Kaede-No-Ki/otakudesu-rest-api) for the inspiration to make this app

Tools I used for making this application:

- node-fetch & cheerio (Web Scrapper). [Tutorial](https://www.youtube.com/watch?v=z6jwIkkc7ro)
- express
- mathjs
- dotenv
- cors
