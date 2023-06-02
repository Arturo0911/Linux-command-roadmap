Perform a **GET** method by defult
==

you can make a simple curl without specificatio the request method"
echo "and by default curl make a GET method
```bash
curl "http://<url address>"
```
When you make a curl wihtout silent specification, you will see the
whole status in the requesting, so you can include the flag -s for
silent mode like this:

```bash
curl -s http://<url address>
```



In the case the url has ssl connections **https**, you have to include the 
flag **-k**

```bash
curl -k https://<url address>
```

Performing a curl with **POST** method, you can use the flag **-x**
and specify the content to send with the flag **-d** and the fields
inside the content like this:


```bash
curl -X POST http://<url address> -d 'value=<the value>&another_value=<the another value>'
```

In the other case that the content of the value should be in 
another format you can specify it using the flag -H for headers
like this:

```bash
curl -X POST http://<url address> -H "Content-Type: application/json" -d '{"value":"<your value>", "another_value":"<your another value>"}'
```
