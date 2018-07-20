# @gurinder/vue-sortable

Inspired by Adam Wathan https://www.youtube.com/watch?v=jR3R_m5FPRc

HTML

```html
<ul slot-scope="{ items }">
    <vue-sortable-item v-for="(document, index) in items" :key="document.id">
        <li>
            <p v-tex="document.title"></p>

            <vue-sortable-handle>
                <button type="button" class="handle">button</button>
            </vue-sortable-handle>
        </li>
    </vue-sortable-item>
</ul>    
```

JS
```JS
import {SortableList, SortableItem, SortableHandle} from '@gurinder/vue-sortable'

Vue.components('sortable-list', SortableList);
Vue.components('sortable-item', SortableItem);
Vue.components('sortable-handle', SortableHandle);
```