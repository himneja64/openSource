<div align="center">
	<h1><a href="https://open-source6-lime.vercel.app/">Multi Slider</a></h1>
	<img src="https://github.com/user-attachments/assets/736034e5-52ce-41a6-850c-dd5fc51da7f5" alt="preview" />
</div>

<br/>

## 🧩사용 기술
![React](https://img.shields.io/badge/react-%2320232a.svg?style=flat-square&logo=react&logoColor=%2361DAFB)
![JavaScript](https://img.shields.io/badge/-JavaScript-dc8d2d?style=flat-square&logo=javascript&logoColor=ffffff)
![Swiper](https://img.shields.io/badge/Swiper-6332F6?style=flat-square&logo=swiper&logoColor=white&style=flat-square)

<br/>

## 💻기능과 특징
> swiper.js

React로 swiper를 적용하고 특정 해상도에 따라 분기하여 시각적 편의성을 제공합니다. 동시에 불필요한 기능이 로딩되는 것을 방지하고, 확장성에 유리합니다.

<br/>

## code
```javascript
import {useState} from 'react';
function Slider(){
	let [device, setDevice]=useState("");

	useEffect(() => {
		window.addEventListener("resize", function(){
			let w=window.innerWidth;

			if(w >= 1024){
				setDevice("desktop");
			}
		});
	}, []);
	if (device === ""){
		return(
			<p>Loading ...</p>
		);
	} else {
		return(
			device === "desktop" ?
			:
		);
	}
}
```
반응형 형식에 따라 DOM을 다르게 그리는 구조로,  
state 상태 값을 사용해 화면 return을 재실행하는 UI를 구현함.

![Footer](https://capsule-render.vercel.app/api?type=waving&color=5f6571&height=100&section=footer)