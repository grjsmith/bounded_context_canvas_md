# Bounded Context Canvas Markdown Template


> Created by: *[Insert name here*] Date: *[Insert data here]*

## Name

>*[Insert name of service here]*

## Description

>*[Describe the value service or context provides and how it provides them]*

## Ubiquitous language

>*[Record any context specific domain terminology]*
>
>- *Domain term: Definition_1*
>- *Domain term: Definition_2*
>- *Domain term: Definition_n*

## Inbound data

### Data provided by other contexts

>*[Describe the data the service is dependent on in order to provide the benefits]*

```yaml
# Data inbound from context1
   key1: value1
     key2: 
       key2a: value2a
       key2b: value2b
     key3: value3
     key4: 
       key4a: value4a
       key4b: value4b
       key4c: value4c
     key5: value5
```

```yaml
# Data inbound from context2
   key1: value1
   List1: ['value2', 'value3', 'value4']
```

### Events consumed

>*[List topics the service listens to and the specific events being consumed]*
>
>- *topic_name_1*
>   - *topic_name_1_event_1*
>   - *topic_name_1_event_2*
>   - *topic_name_n_event_n*

## Business rules

> *[Describe the logic the service contains. Describe actions it performs when the service receives a `query`, `command` or `event`.]*

1. GIVEN `topic_name1_event1` occurs WHEN `key1 = value1` THEN do `action1`

## Outbound Data

```yaml
# Data outbound to context4
    key6: value6
```

## Events published

>*[List topics the service listens to and the specific events being consumed]*
>
>- *topic_name_2*
>   - *topic_name_2_event_1*
>   - *topic_name_2_event_2*
>   - *topic_name_n_event_n*

## Assumptions

> *[List the assumptions made by the service or bounded context itself or made by the team building the service]*
>
>- *topic_name1_event1 only occurs when some real world event occurs*
