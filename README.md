# Elastic Galaxy Tools

* [What are Elastic Galaxy Tools](#what-are-elastic-galaxy-tools?)
* [How to use Elastic Galaxy Tools](#how-to-use-elastic-galaxy-tools?)
* [How to develop an Elastic Galaxy Tool](#how-to-develop-an-elastic-galaxy-tool?)
    + [Publish a Galaxy Tool](#publish-a-galaxy-tool)




## What are Elastic Galaxy Tools?

Elastic Galaxy tools is a type of Galaxy tools that have elastic user interfaces. Users can adjust the
number of input fields a tool can have.

## How to use Elastic Galaxy Tools?

## How to develop an Elastic Galaxy Tool?

### Publish a Galaxy tool

We can use the tool **planemo** to easily publish our Galaxy tools to Tool Shed or test Tool Shed. 
More details can be found **[here](http://planemo.readthedocs.io/en/latest/publishing.html)**.

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



