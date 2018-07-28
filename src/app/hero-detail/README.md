
# the thing that we did in this branch
* You simplified the HeroesComponent by reducing its responsibilities.

* You can evolve the HeroDetailComponent into a rich hero editor without touching the    
  parent HeroesComponent.

* You can evolve the HeroesComponent without touching the hero detail view.

* You can re-use the HeroDetailComponent in the template of some future component.

# new things that we learn
## @input decorator
we imported the hero class and bind it with input decorator like this:

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
