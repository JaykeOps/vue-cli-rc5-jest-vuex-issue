# Steps to reproduce

## Project setup

### Clone 
then run `npm run test:unit`

### Alternatively
With @vue/cli rc5
```
vue create <project-name>

```

**select:**

```
Typescript
Vuex
Jest
```

After install replace `/tests/HelloWorld.spec.ts` content with:
```
import { shallowMount } from '@vue/test-utils'
import HelloWorld from '@/components/HelloWorld.vue'
import store from "@/store";

describe('HelloWorld.vue', () => {
  it('renders props.msg when passed', () => {
    store.state;
  })
})
```
**Run** `npm run test:unit`
