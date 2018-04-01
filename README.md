# Elastic Galaxy Tools

* [What are Elastic Galaxy Tools](#what-are-elastic-galaxy-tools?)
* [How to use Elastic Galaxy Tools](#how-to-use-elastic-galaxy-tools?)
* [How to develop an Elastic Galaxy Tool](#how-to-develop-an-elastic-galaxy-tool?)
    + [Publish a Galaxy Tool](#publish-a-galaxy-tool)




## What are Elastic Galaxy Tools?

**Elastic Galaxy tools** is a type of Galaxy tools that have elastic user interfaces. Users can adjust the
number of input fields a tool can have, just like using a command line tool. When using a command line tool,
users can choose which (non-required) options to use. I hope Galaxy users can do the same thing, but without
actually writing any command line scripts.
 

## How to use Elastic Galaxy Tools?

Although any (Elastic) Galaxy tool is a wrapper of a command line tool which enables performing data analysis
through web interfaces without actually writing any command line script, understanding how to read command line
manuals will help you use Elastic Galaxy tools. 

Running a command line tool is very simple. You start with the tool name, then you specify options (also called flags) 
that the tool can recognize. The tool manual should tell you which options the tool can recognize. An option may or may 
not have a value followed. Some options are required and some are optional. You have to use all required options to 
successfully run a command line tool. However, you can use as many optional options as you want in a call of a command 
line tool.

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



