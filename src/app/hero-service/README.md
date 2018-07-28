
# the thing that we did in this branch
* 

* 

* 

* 

# new things that we learn
## @injectable decorator
* This marks the class as one that participates in the dependency injection system. 

* HeroService class is going to provide an injectable service, and it can also have its  own injected dependencies. 

```
@Input() hero: Hero;

```

The Hero property must be an Input property, 
because the external HeroesComponent will bind to it like this.
```
<app-hero-detail [hero]="selectedHero"></app-hero-detail>

```
where
<app-hero-detail> is hero detail component selector 
[hero]="selectedHero" is the hero data that is being parsed by heroes component when the heroes are being selected

# in a nut shell
this hero-details-component work as html template that took selected hero data from heroes component and show the the data through hero-details-component.html 
