# <p align="center">AngularMaterial 🕹 </p> 

# <p align="center"> Estructura básica  ![angular](https://user-images.githubusercontent.com/71487857/212993270-3cf1454e-f0d7-4164-bc01-20d5fe6469cd.png)Angular Material Mobile![androide36](https://user-images.githubusercontent.com/71487857/228891500-07e27fa3-edc3-4838-8c56-ba78673a3367.jpg) App with  ![descarga](https://user-images.githubusercontent.com/71487857/212993697-6234ef26-0e4a-40ce-bc8a-a9bfa858a74b.png)Capacitor</p>

## URL
* Angular
```
https://angular.io/start
```
* Angular Material
```
https://material.angular.io/
```
* schematics
```
https://material.angular.io/guide/schematics
```
## Creo el nuevo proyecto scss:
```
ng new AngularMaterial --routing --style=scss
```
```
cd .\AngularMaterial\
```
```
ng add @angular/material
- Would you like to proceed? (Y/n)yes
```
```
> Purple/Green       [ Preview: https://material.angular.io?theme=purple-green ]
```
```
 Set up global Angular Material typography styles? Yes
 ```
 ```
 Include the Angular animations module? yes
 ```
 * Levantar app
```
 ng serve -o
 ```
* App navigator
```
ng g @angular/material:navigation app-navigation
```
* Vamos a src\app\app.component.html
 - Borramos todos y añadimos el componente navigator:
 ```
 <app-app-navigation></app-app-navigation>
 ```
