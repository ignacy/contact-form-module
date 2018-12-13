## Contact Form Module

Concat form module for your page after installation can be used directly from
`contact_form/messages` and `contact_form/new_message` URI's or it can be inlcluded as:

1. Regular form

for example:

```liquid
{% include_form 'modules/contact_form/message', parent_resource_id: "message" %}
```


2. Partial exporting variables

```liquid
{% include 'modules/contact_form/messages' %}
# exports list of messages in context:
{{ context.exports.contact_form.messages }}
```
