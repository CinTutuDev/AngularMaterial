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
* Capactor
```
https://capacitorjs.com/
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
* Crear componente 
```
ng g component about
```
* crear dashboard (Panel)
```
ng g @angular/material:dashboard panel
```
## Creo las Path en app-routing.module.ts
```
const routes: Routes = [
  {
    path: '',
    children: [
      {
        path: '',
        component: PanelComponent
      },
      {
        path: 'about',
        component: AboutComponent
      },
      {
        path: '404',
        component: ErrorComponent
      },
      {
        path: '**',
        redirectTo: '404',
      }
    ]
  }
];
```
## Para añadir el panel o DAshboard al pg de inicio \app-navigation\app-navigation.component.html
```
  <router-outlet></router-outlet>
```
## Antes de añdir Capacitor hago build
```
ng build
```
## Instalar Capacitor
```
 npm install @capacitor/cli --save-dev
 npx cap init
```
## Para instalar ios/android
```
npm install @capacitor/ios @capacitor/android
npx cap add android
npx cap add ios
```
* 👀Error❗❗
[error] The web assets directory (.\dist) must con......<br>
[error] Error: ENOENT: no such file or director.........<br>
* Ir capacitor.config.ts
```
const config: CapacitorConfig = {
❗❗donde esta el dist:
 ❌ webDir: 'dist',
 
};
const config: CapacitorConfig = {
❗❗donde esta el dist PONER el nombre del proyecto como vien en el dist:
 ✔ webDir: 'dist/angular-material',
};

```


