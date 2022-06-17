# Welcome to my GitHub Pages 👋🏻
In this website you can see my online interest provided with link source.

Find me also on:
[Linkedin](https://www.linkedin.com/in/deta-u-8bb1a7107/) |
[Instagram](https://www.instagram.com/deta_utama/) | 
[Stack Overflow](https://stackoverflow.com/users/7207817/deta-utama) |
[Oddbit.id](https://oddbit.id) 

Search with tag: #Web, #Github, #PortfolioWebsite, #Documentation, #React, #NextJs, #Devtools, #Geolocation

## 📌 My new personal website
<sup>00:45, Friday, June 17, 2022 (GMT+8). Time in Celuk, Gianyar Regency, Bali</sup> <br />
I have been created personal website using my own domain. But I take it down because I think it will not useful because it only provide like card name. And not suitable with cost of domain 💰. So I will try to use this github pages with concept "My Programming Diary". I will post my activity here like a bookmark and hopefully will be useful for other too 🙂. Also I don't want to confused about code and design of the website 😆. <br />
`#Web #Github #PortfolioWebsite`

## How to know when user entered an area in map
I'm working on web game project using user device location and map, when user position (geolocation) entered an area in map. They will got point
```
// import booleanPointInPolygon from "@turf/boolean-point-in-polygon";

// state.spots[index].area: Feature<Polygon, {
//   spotId: string;
//   points: number;
// }>

const found = booleanPointInPolygon(
  state.userPosition,
  area
);
```
`#React #Turf #Leaflet`

## This is how I avoid multiple rendering when geolocation callback triggered more than once
<sup>15:12 Friday, June 17, 2022 (GMT+8) Time in Dangin Puri Klod, Denpasar City, Bali</sup> <br />
Why? [Demo](https://codesandbox.io/s/affectionate-tdd-mrygkx?file=/src/App.js) <br />
Solution: 
```
// Get user location
  useEffect(() => {
    navigator.geolocation.watchPosition((pos) => {
      console.log("Changed position");
      if (
        _userPosition !== point([pos.coords.longitude, pos.coords.latitude])
      ) {
        _setUserPosition(point([pos.coords.longitude, pos.coords.latitude]));
      }
    });
    // eslint-disable-next-line react-hooks/exhaustive-deps
  }, []);
 ```
`#React #NextJs #Geolocation`

## TIL: I thought my code is the problem about "Why it rendered twice?".
<sup>01:43 Friday, June 17, 2022 (GMT+8) Time in Celuk, Gianyar Regency, Bali</sup> <br />
Until I realize that  if you don't install React DevTools extension in your browser, it will show like the web rendered twice (first snip). And then if you installed React DevTools in your browser, it will show you the second rendered is from the DevTools (second snip). 
Another reference: [Next dev with React 18, Always render twice](https://github.com/vercel/next.js/issues/35822)<br/>
![Snip log](https://raw.githubusercontent.com/detautama/detautama.github.io/main/images/image.png) <br/>
`#React #NextJs #Devtools`

## Mardkown Badges
<sup>01:33, Friday, June 17, 2022 (GMT+8), Time in Celuk, Gianyar Regency, Bali</sup> <br />
Markdown badges, I think I it will be useful for documentation
[Mardkown Badges](https://ileriayo.github.io/markdown-badges/#markdown-badges) <br/>
`#Web #Github #PortfolioWebsite #Documentation`
