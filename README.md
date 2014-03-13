## HTML

bbform

```html
<form class="bb-bundle-form" data-action="${1:namespace}">
    ${2}
</form>
```

bblink
```html
<a class="bb-bundle-link" data-href="${1:namespace}">${2:text}</a>
```

## JS

req
```javascript
bb.require(['bb.BundleController'], function () {
    ${1}
});
```

act
```javascript
bb.bundle.addAction('${1:namespace}', {
    params: function () {
        return ${2:{}};
    },
    success: function (response) {
        ${3}
    }
});
```

reqact
```javascript
bb.require(['bb.BundleController'], function () {
    bb.bundle.addAction('${1:namespace}', {
        params: function () {
            return ${2:{}};
        },
        success: function (response) {
            ${3}
        }
    });
});
```

##php

bundle
create the minimal structure for bundle entry point