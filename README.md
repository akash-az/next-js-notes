# next-js-notes

** How to make sure website takes 3 sec loading time 

```next
async function takeTime(){

  await new Promise((resolve) => {
    setTimeout(resolve,3000);
 }

);

}

export default async function Home() {
 await takeTime();
    return (
    <div>
      <h1>
        This is the home page
      </h1>

    </div>
  );
}
```


## creating apis in nect js

if w e create any file in app folder with the name route.js it will be treated as an API
