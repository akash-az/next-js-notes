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


## creating apis in next js

* if we create any file in app folder with the name route.js it will be treated as an API
** we can accept dynamic values from url variable , body, query param 

