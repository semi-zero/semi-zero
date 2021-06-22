# Dillinger
## _The Last Markdown Editor, Ever_

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Dillinger is a cloud-enabled, mobile-ready, offline-storage compatible,
AngularJS-powered HTML5 Markdown editor.

- Type some Markdown on the left
- See HTML in the right
- ✨Magic ✨

## Profile

- 성균관대학교 유학동양학/통계학 졸업
- 성균관대학교 데이터사이언스융합대학원 재학
- Email: dpapfkfemha@gmail.com

## Career

- 데이콘 _2020.06~_
  - AI Hackathon 설계, 운영 평가
  - AI 교육 강사

## Hackathon Development

경진대회 설계, 운영 리스트

### Public Hackathon 

- [심리 성향 예측 AI 경진대회](https://www.dacon.io/competitions/official/235647/overview/description)
- [딥페이크 변조 영상 탐지 AI 경진대회] - awesome web-based text editor
- [소설 작가 분류 AI 경진대회] - Markdown parser done right. Fast and easy to extend.
- [AI야, 진짜 뉴스를 찾아줘! AI 경진대회] - great UI boilerplate for modern web apps
- [Y&Z세대 투자자 프로파일링 시각화 경진대회] - evented I/O for the backend
- [국회 입법활동 빅데이터 시각화 경진대회] - fast node.js network app framework [@tjholowaychuk]
- [운동 동작 분류 AI 경진대회] - the streaming build system
- [제 2회 컴퓨터 비전 학습 경진대회](https://breakdance.github.io/breakdance/) - HTML
- [신용카드 사용자 연체 예측 AI 경진대회] - duh
- [로그 분석을 통한 보안 위험도 예측 AI 경진대회]
- [전력사용량 예측 AI 경진대회]
- [자연어 기반 기후기술분류 AI 경진대회]

And of course Dillinger itself is open source with a [public repository][dill]
 on GitHub.

## Installation

Dillinger requires [Node.js](https://nodejs.org/) v10+ to run.

Install the dependencies and devDependencies and start the server.

```sh
cd dillinger
npm i
node app
```

For production environments...

```sh
npm install --production
NODE_ENV=production node app
```

## Plugins

Dillinger is currently extended with the following plugins.
Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantaneously see your updates!

Open your favorite Terminal and run these commands.

First Tab:

```sh
node app
```

Second Tab:

```sh
gulp watch
```

(optional) Third:

```sh
karma test
```

#### Building for source

For production release:

```sh
gulp build --prod
```

Generating pre-built zip archives for distribution:

```sh
gulp build dist --prod
```

## Docker

Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the
Dockerfile if necessary. When ready, simply use the Dockerfile to
build the image.

```sh
cd dillinger
docker build -t <youruser>/dillinger:${package.json.version} .
```

This will create the dillinger image and pull in the necessary dependencies.
Be sure to swap out `${package.json.version}` with the actual
version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on
your host. In this example, we simply map port 8000 of the host to
port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart=always --cap-add=SYS_ADMIN --name=dillinger <youruser>/dillinger:${package.json.version}
```

> Note: `--capt-add=SYS-ADMIN` is required for PDF rendering.

Verify the deployment by navigating to your server address in
your preferred browser.

```sh
127.0.0.1:8000
```

## License

MIT

**Free Software, Hell Yeah!**

<!--
**semi-zero/semi-zero** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
