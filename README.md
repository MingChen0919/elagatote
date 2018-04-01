# Elastic Galaxy Tools

## What is Elastic Galaxy Tools?

Elastic Galaxy tools is a type of Galaxy tools that have elastic user interfaces. Users can adjust the
number of input fields a tool can have.

## How to use Elastic Galaxy Tools?

## How to develop Elastic Galaxy Tools?

### Publish a Galaxy tool

We can use the tool **planemo**. More details can be found **[here](http://planemo.readthedocs.io/en/latest/publishing.html)**.

* Publish to test Tool Shed

```bash
planemo shed_create --shed_target testtoolshed
``` 

* Update tool repository in test Tool Shed

```bash
planemo shed_update --check_diff --shed_target testtoolshed
```

* Publish to Tool Shed

```bash
planemo shed_create --shed_target toolshed
```

* Update tool repository in Tool Shed

```bash
planemo shed_update --check_diff --shed_target toolshed
```



