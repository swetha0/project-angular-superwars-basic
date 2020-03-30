![Image description](https://i1.faceprep.in/ProGrad/face-logo-resized.png)

# ProGrad Lab | Superwars Stage 2

Remember Superwars stage 1? However, here is a quick recap of things.

Dustin and Lucus are best friends. They spend their weekends watching superhero series and playing superhero games. One Friday at school Mr.Hooper, their computer science faculty taught them HTML, CSS, and JavaScript. Dustin & Lucus realised they could build super cool super hero stuff using their knowledge. 

The subsequent weekend, they decided to do it. Lucus and Dustin are now all set to build something super cool.

Lucus always loves protagonists like most of us. But Dustin is quite crazy, he likes antagonists. So they decided to collect a bunch of their favorite Super Heroes and Super Villains names along with their pictures. Did they tell you about the game that they are gonna build? 

Okay, let us explain. They are going to facilitate the ultimate war between Super Heroes and Super Villains. As they are new to these technologies, they need a **ProGrad** to help them build this game.

## Learning Goals

After this lesson, you will be able to:

- Create a static Angular application with Angular CLI.
- Build an Angular application with one component.

## Requirements

- Fork this repo.
- Clone this repo.

## Submission

Upon completion, run the following commands:

```bash
$ git add .
$ git commit -m "done"
$ git push origin master
```

Navigate to your repo and create a pull request from your master branch to the original repository's master branch.

In the pull request name, add your Prograd id, name, and last name separated by a dash "-".

## Deliverables

You need to generate the starter code and fill it with the necessary code to satisfy the requirements described below.

## Starter code

You need to create an array of 20 Super Heroes and Super-Villains. We are talking about the array of 20 _strings_ containing each Super Heroes and Super-Villains names. Here is one example of how the data is displayed:

```javascript
[
    "Spiderman"
]
```


### Progression 1: More players, more fun

Dustin and Lucus wants to create players.In `initPlayers()`, loop through passed constant and  create JSON Objects, such that each player contains name, strength, image url and type.  
* Use default `strength` as any number.  
* `image` can be sequential i.e. "images/super-"+(i+1)+".png"  
* `type` of player can alternating between hero and villain or your own logic
* It should _return an array_ of player objects.
    ```javascript
    [
        {
            name:"Super Man",
            strength:100,
            image:"images/hero-1.png",
            type:"hero|villain"
        }
    ]
    ```

### Progression 2: Courage is grace

Add your logic in `getRandomStrength()` method, such that it should _return a random strength_ from 1 to 100. The strength is what is gonna decide the winner.

### Progression 3: No player should fall

In `buildPlayers()`, loop through the created JSON objects and accumulate HTML template as below and _return HTML element_.
 ```JS
<div class="player">
    <img src="${players[i].image}">
    <div class="name">${players[i].name}</div>
    <div class="strength">${players[i].strength}</div>
</div>
```

## Expected Output

![Superwars](https://github.com/FACEPrep-ProGrad/project-12-superwars-basic/raw/master/doc/superwars-basic1.png)
![Superwars](https://github.com/FACEPrep-ProGrad/project-12-superwars-basic/raw/master/doc/superwars-basic2.png)

Happy Coding ProGrad ❤️
