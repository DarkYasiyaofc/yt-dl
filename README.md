## 📝 Table of Contents

- [About](#about)
- [Usage](#usage)
- [Authors](#authors)

## 🧐 About <a name = "about"></a>

A simple YouTube video downloader for audio and video formats.

### Installing


```sh
yarn add @dark-yasiya/yt-dl.js
```

or

```sh
npm i @dark-yasiya/yt-dl.js
```

## 🍟 Usage <a name="usage"></a>

```ts
const { ytsearch, ytmp3, ytmp4 } = require('@dark-yasiya/ytdl.js')
```


## Yt Search

```ts
const text = "lelena";
const result = ytsearch(text);
console.log(result);
```
```ts
{
  result: true,
  creator: '@DarkYasiya',
  results: [
    {
      type: 'video',
      videoId: '0geqOYqwL0s',
      url: 'https://youtube.com/watch?v=0geqOYqwL0s',
      title: 'Lelena (ලෙලෙනා) - Nilan Hettiarachchi Official Music Video',
      description: 'Title | Lelena Artiste | Nilan Hettiarachchi Music Produced by Chamath Sangeeth Lyrics | Dulan ARX ( Dulanja Alwis) Directed by ...',
      image: 'https://i.ytimg.com/vi/0geqOYqwL0s/hq720.jpg',
      thumbnail: 'https://i.ytimg.com/vi/0geqOYqwL0s/hq720.jpg',
      seconds: 195,
      timestamp: '3:15',
      duration: [Object],
      ago: '3 years ago',
      views: 37740125,
      author: [Object]
    },
    {
      type: 'video',
      videoId: 'AFqtArWpv-w',
      url: 'https://youtube.com/watch?v=AFqtArWpv-w',
      title: 'Nilan Hettiarachchi - ලෙලෙනා | Lelena (Lyrics)',
      description: 'Title | Lelena Artiste | Nilan Hettiarachchi Music Produced by Chamath Sangeeth Lyrics | Dulan ARX ( Dulanja Alwis) Directed by ...',
      image: 'https://i.ytimg.com/vi/AFqtArWpv-w/hq720.jpg',
      thumbnail: 'https://i.ytimg.com/vi/AFqtArWpv-w/hq720.jpg',
      seconds: 194,
      timestamp: '3:14',
      duration: [Object],
      ago: '3 years ago',
      views: 529654,
      author: [Object]
    },
    {
      type: 'video',
      videoId: 'qcKQCymbXWE',
      url: 'https://youtube.com/watch?v=qcKQCymbXWE',
      title: 'ලෙලෙනා - Lelena | Nilan Hettiarachchi song | Chipmunks & Himabole version song with lyrics',
      description: 'lelena Himabole Studio Thanks for watching ❤ Like Comment Share.',
      image: 'https://i.ytimg.com/vi/qcKQCymbXWE/hq720.jpg',
      thumbnail: 'https://i.ytimg.com/vi/qcKQCymbXWE/hq720.jpg',
      seconds: 169,
      timestamp: '2:49',
      duration: [Object],
      ago: '3 years ago',
      views: 1760313,
      author: [Object]
    } ... more results
  ]
}
```

## Download Ytmp3
```ts
const yturl = "https://www.youtube.com/watch?v=vOv2i88NmA4";
const result = ytmp3(yturl);
console.log(result);
```
```ts
{
  status: true,
  creator: '@DarkYasiya',
  result: {
    type: 'video',
    videoId: 'vOv2i88NmA4',
    url: 'https://youtube.com/watch?v=vOv2i88NmA4',
    title: 'Age Sinahawa Thahanam | ඇගෙ සිනහව තහනම් | Vini Productions - විනී',
    description: 'Age Sinahawa Thahanam | ඇගෙ සිනහව තහනම් | Vini Productions - විනී ✓1XBET MELBET ගහලා ...',
    image: 'https://i.ytimg.com/vi/vOv2i88NmA4/hq720.jpg',
    thumbnail: 'https://i.ytimg.com/vi/vOv2i88NmA4/hq720.jpg',
    seconds: 1541,
    timestamp: '25:41',
    duration: {
      toString: [Function: toString],
      seconds: 1541,
      timestamp: '25:41'
    },
    ago: '2 days ago',
    views: 2003354,
    author: {
      name: 'Vini Productions - විනී',
      url: 'https://youtube.com/@viniproductionsofficial'
    }
  },
  download: {
    quality: 'mp3',
    availableQuality: [
      'mp3',  'm4a',
      'webm', 'acc',
      'flac', 'opus',
      'ogg',  'wav',
      '4k'
    ],
    url: 'https://bessie88.oceansaver.in/pacific/?J3WI8gne3gqO2qQ7IbZMakw',
    filename: 'Age Sinahawa Thahanam | ඇගෙ සිනහව තහනම් | Vini Productions - විනී.mp3'
  }
}
```

## Download Ytmp4

```ts
const yturl = "https://www.youtube.com/watch?v=vOv2i88NmA4";
const quality = "360p";
const result = ytmp4(yturl, quality);
console.log(result);
```
```ts
{
  status: true,
  creator: '@DarkYasiya',
  result: {
    type: 'video',
    videoId: 'vOv2i88NmA4',
    url: 'https://youtube.com/watch?v=vOv2i88NmA4',
    title: 'Age Sinahawa Thahanam | ඇගෙ සිනහව තහනම් | Vini Productions - විනී',
    description: 'Age Sinahawa Thahanam | ඇගෙ සිනහව තහනම් | Vini Productions - විනී ✓1XBET MELBET ගහලා ...',
    image: 'https://i.ytimg.com/vi/vOv2i88NmA4/hq720.jpg',
    thumbnail: 'https://i.ytimg.com/vi/vOv2i88NmA4/hq720.jpg',
    seconds: 1541,
    timestamp: '25:41',
    duration: {
      toString: [Function: toString],
      seconds: 1541,
      timestamp: '25:41'
    },
    ago: '2 days ago',
    views: 2005666,
    author: {
      name: 'Vini Productions - විනී',
      url: 'https://youtube.com/@viniproductionsofficial'
    }
  },
  download: {
    quality: 360,
    availableQuality: [
      '144',  '240',
      '360',  '480',
      '720',  '1080',
      '1440'
    ],
    url: 'https://carl89.oceansaver.in/pacific/?Fp8tZWSaFLBxdoyy08bKkra',
    filename: 'Age Sinahawa Thahanam | ඇගෙ සිනහව තහනම් | Vini Productions - විනී (360p).mp4'
  }
}
```

## 🖋 Authors <a name = "authors"></a>

- [@DarkYasiya](https://github.com/DarkYasiyaofc) - scraped author
