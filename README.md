# vue-inline-jalaali-calender
[moment-jalaali](https://www.npmjs.com/package/moment-jalaali) and [bootstrap](https://getbootstrap.com/docs/4.3/getting-started/introduction/) have been used to create this component.


## page
* [Home page](https://mohammadrezaei0123.github.io/vue-inline-jalaali-calender/)
* [Relative Component](https://www.npmjs.com/package/vue-inline-calender)

## Installation CDN:
```html
<link rel="stylesheet"https://unpkg.com/vue-inline-jalaali-calender@latest/dist/v-inline-jalaali-calender.css">
<script src="https://unpkg.com/vue-inline-jalaali-calender@latest/dist/v-inline-jalaali-calender.common.js"></script>
```

## Installation npm:
```bash
 npm i vue-inline-jalaali-calender --save
```

## Components
* InlineCalender
* InlineCalenderVertical
* MonthCalender
* YearCalender
* TenYearCalender
* FullCalender
* FullCalenderVertical

### add style
main.js
```bash
import 'vue-inline-jalaali-calender/dist/v-inline-jalaali-calender.css'
```
## sample

```html
<template>
    <InlineCalender
        v-bind="{
        useRaitoSizing: false,
        mainBodyStyle: e1.mainBodyStyle,
        afterTodayStyle: e1.afterTodayStyle,
        titleStyle: e1.titleStyle,
        beforeTodayStyle: e1.beforeTodayStyle,
        rowCalenderStyle: e1.rowCalenderStyle,
        headerCalenderStyle: e1.headerCalenderStyle,
        footerStyle: e1.footerStyle,
        todayStyle: e1.todayStyle,
        todayButtonStyle: e1.todayButtonStyle,
        showSelectedValueStyle: e1.showSelectedValueStyle
        }"
    />
</template>

<script>
import {InlineCalender} from "v-inline-jalaali-calender";
export default {
    components:{InlineCalender},
    data(){
        return{
            e1: {
                mainBodyStyle: {
                width: "300px",
                background: "#eaffd0",
                border: "2px solid #311d3f",
                borderRadius: "5px",
                padding: "15px"
                },
                titleStyle: {
                height: "40px",
                marginBottom: "5px",
                color: "#88304e"
                },
                headerCalenderStyle: {
                height: "40px",
                color: "#fff",
                background: "#88304e",
                margin: "0 -14.5px"
                },
                rowCalenderStyle: {
                height: "50px",
                margin: "0 -14px"
                },
                footerStyle: {
                height: "20px",
                color: "#88304e"
                },
                afterTodayStyle: {
                color: "#eeeeee",
                boxShadow: "inset 0 0 10px #311d3f",
                background: "#88304e",
                transition: "all 1s"
                },
                todayStyle: {
                color: "#eeeeee",
                background: "#522546",
                boxShadow: "0 0 5px #eeeeee",
                transition: " all 1s"
                },
                beforeTodayStyle: {
                background: "#eeeeee",
                boxShadow: "inset 0 0 10px #88304e",
                color: "#88304e",
                transition: "all 1s"
                },
                todayButtonStyle: {
                color: "#88304e"
                },
                showSelectedValueStyle: {
                display: "flex",
                alignItems: "center",
                color: "#88304e"
                }
            },
        }
    }
}
</script>
```
