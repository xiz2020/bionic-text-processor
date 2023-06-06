# bionic-text-processor
**Description** 

Bionic Reading - is a shallow method of reading facilitating the reading process by guiding the eyes through text with artificial fixation points. As a result, the reader is only focusing on the highlighted initial letters and lets the brain center complete the word.

**API:** 

https://rapidapi.com/zilinskivan/api/fast-reading

**Example:**

![image](https://20fix.com/xtext/t.jpg)

**Code Samples:** 

**-HTTP**

<pre>
GET /api/?txt=Fast%20Reading%20-%20is%20a%20shallow%20method%20of%20reading%20facilitating%20the%20reading%20process%20by%20guiding%20the%20eyes%20through%20text%20with%20artificial%20fixation%20points.%20As%20a%20result%2C%20the%20reader%20is%20only%20focusing%20on%20the%20highlighted%20initial%20letters%20and%20lets%20the%20brain%20center%20complete%20the%20word.&lng=en&fix=5&model=m1 HTTP/1.1
X-Rapidapi-Key: Your API Key
X-Rapidapi-Host: fast-reading.p.rapidapi.com
Host: fast-reading.p.rapidapi.com
</pre>

**-Javascript**

<pre>
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener('readystatechange', function () {
	if (this.readyState === this.DONE) {
		console.log(this.responseText);
	}
});

xhr.open('GET', 'https://fast-reading.p.rapidapi.com/api/?txt=Fast%20Reading%20-%20is%20a%20shallow%20method%20of%20reading%20facilitating%20the%20reading%20process%20by%20guiding%20the%20eyes%20through%20text%20with%20artificial%20fixation%20points.%20As%20a%20result%2C%20the%20reader%20is%20only%20focusing%20on%20the%20highlighted%20initial%20letters%20and%20lets%20the%20brain%20center%20complete%20the%20word.&lng=en&fix=5&model=m1');
xhr.setRequestHeader('X-RapidAPI-Key', 'Your API Key');
xhr.setRequestHeader('X-RapidAPI-Host', 'fast-reading.p.rapidapi.com');

xhr.send(data);
</pre>

**-PHP**

<pre>
<?php

$curl = curl_init();

curl_setopt_array($curl, [
	CURLOPT_URL => "https://fast-reading.p.rapidapi.com/api/?txt=Fast%20Reading%20-%20is%20a%20shallow%20method%20of%20reading%20facilitating%20the%20reading%20process%20by%20guiding%20the%20eyes%20through%20text%20with%20artificial%20fixation%20points.%20As%20a%20result%2C%20the%20reader%20is%20only%20focusing%20on%20the%20highlighted%20initial%20letters%20and%20lets%20the%20brain%20center%20complete%20the%20word.&lng=en&fix=5&model=m1",
	CURLOPT_RETURNTRANSFER => true,
	CURLOPT_ENCODING => "",
	CURLOPT_MAXREDIRS => 10,
	CURLOPT_TIMEOUT => 30,
	CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
	CURLOPT_CUSTOMREQUEST => "GET",
	CURLOPT_HTTPHEADER => [
		"X-RapidAPI-Host: fast-reading.p.rapidapi.com",
		"X-RapidAPI-Key: Your API Key"
	],
]);

$response = curl_exec($curl);
$err = curl_error($curl);

curl_close($curl);

if ($err) {
	echo "cURL Error #:" . $err;
} else {
	echo $response;
}
</pre>
