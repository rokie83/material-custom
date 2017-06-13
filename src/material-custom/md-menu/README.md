### Simple Menu
```html
<button type="button" tabindex="-1" md-icon-button [mdMenuTriggerFor]="simpleMenu">
    <!-- For the use of custom icons at Bexio until material guys will document how to use md-icon with custom src -->
    <img src="assets/icons/contextmenu-icon.svg" alt="menu-trigger">
</button>
<md-menu #simpleMenu="mdMenu" [overlapTrigger]="false">
    <button md-menu-item>
        <span>Simple Menu Item</span>
    </button>
    <button md-menu-item disabled>
        <span>Disabled Menu Item</span>
    </button>
    <button md-menu-item>
        <span>Simple Menu Item with a very very long text</span>
    </button>
</md-menu>
```

### Contextual Menu
```html
<button type="button" tabindex="-1" md-icon-button [mdMenuTriggerFor]="contextualMenu">
    <!-- For the use of custom icons at Bexio until material guys will document how to use md-icon with custom src -->
    <img src="assets/icons/contextmenu-icon.svg" alt="menu-trigger">
</button>
<md-menu #contextualMenu="mdMenu" class="context-menu-panel" [overlapTrigger]="false">
    <div class="context-menu-item">
        <div class="main-action">
            <button md-menu-item>
                Simple contextual Menu Item
            </button>
        </div>
        <div class="sub-action">
            <button md-icon-button>
                <md-icon fontSet="fa" fontIcon="fa-trash"></md-icon>
            </button>
        </div>
    </div>
    <div class="context-menu-item">
        <div class="main-action">
            <button md-menu-item disabled>
                Disabled contextual Menu Item
            </button>
        </div>
        <div class="sub-action">
            <button md-icon-button disabled>
                <md-icon fontSet="fa" fontIcon="fa-trash"></md-icon>
            </button>
        </div>
    </div>
    <div class="context-menu-item">
        <div class="main-action">
            <button md-menu-item>
                Contextual Menu Item with a very very long text
            </button>
        </div>
        <div class="sub-action">
            <button md-icon-button>
                <md-icon fontSet="fa" fontIcon="fa-trash"></md-icon>
            </button>
        </div>
    </div>
</md-menu>
```
