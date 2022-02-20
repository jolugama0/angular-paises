# PaisesApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Qué se aprende?

- Uso de bootstrap como css framework (cargado en el index.html)
- links con routerLink en sidebar y por-pais.component. 
- output y eventEmitter, input, en pais-input.component. Para ello se importa `RouterModule` en pais.module y shared.module
- rxjs, como debounceTime en pais-input.component 
- Ejemplo de input, con [(ngModel)] en pais-input.component. Cargando en su módulo (país.module) FormsModule

```html
<form (ngSubmit)="buscar()" autocomplete="off">
    <input type="text"
           name="termino"
           class="form-control"
           [(ngModel)]="termino"
           (input)="teclaPresionada()"
           [placeholder]="placeholder"/>
</form>

```

- Servicio con pais.service. Uso de HttpClient, HttpParams
- switchMap, para no meter un subscribe dentro de otro subscribe. Un observable que devuelve otro observable. 
