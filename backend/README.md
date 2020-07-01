{
	"variables": [],
	"info": {
		"name": "udacity-fsnd-udaspicelatte",
		"_postman_id": "fa3eaf73-b2a5-124d-cf16-ce765c21d607",
		"description": "",
		"schema": "https://schema.getpostman.com/json/collection/v2.0.0/collection.json"
	},
	"item": [
		{
			"name": "public",
			"description": "",
			"item": [
				{
					"name": "/drinks",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 200\", function () {",
									"    pm.response.to.have.status(200);",
									"});",
									"",
									"pm.test(\"value contains drinks array\", function () {",
									"    var jsonData = pm.response.json();",
									"    pm.expect(jsonData.drinks).to.be.an('array')",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks",
						"method": "GET",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": ""
						},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks-detail",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 401\", function () {",
									"    pm.response.to.have.status(401);",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks-detail",
						"method": "GET",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": ""
						},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 401\", function () {",
									"    pm.response.to.have.status(401);",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks",
						"method": "POST",
						"header": [
							{
								"key": "Content-Type",
								"value": "application/json",
								"description": ""
							},
							{
								"key": "Authorization",
								"value": "Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ill1Y0NnYU5XaDh4SWttcnpXUEltRCJ9.eyJpc3MiOiJodHRwczovL215Y29mZmVlYXBpLnVzLmF1dGgwLmNvbS8iLCJzdWIiOiJhdXRoMHw1ZWZhOWUzMzcxNDY4YzAwMTNmZmJiOGIiLCJhdWQiOiJDb2ZmZWUiLCJpYXQiOjE1OTM1NDk1MDksImV4cCI6MTU5MzU0OTU2OSwiYXpwIjoiTjJJRDZBMmZnWHBKZnBYdTA2WWFnQTBZZ2YwMjBHdTkiLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbImdldDpkcmlua3MtZGV0YWlsIiwicG9zdDpkcmlua3MiXX0.0bDzX4mUb0JXkCvRzadEu1ejoV2fcpPjk89jucC09vEHRYpN5wJFhO7GdAxAFRyXwOL4prTODrCzAIeevjhdfOMsCPsKMHcrBw-tk-4zjr9kXjNbXtQPGPID5thc2I0vURsp5f1qAYHAHyamEHRLBvnNjo6VkoSuW33wAHAPcSW_DcP8CyWabm6S1ib8u_3Galfm88bTUboW2RyBLqSricYXxJzCGu7tfLLF-T3JA4nG58R-akTJUSOQx3QnfwOVTHIPROy0tBvK3IrMOQAjD9wZrbfCOipBmg5TJGG7rbsqs_p-GnzUJ7HQOiXQVGqREn6posJVwTzcDMTU4jheOQ",
								"description": "",
								"disabled": true
							}
						],
						"body": {
							"mode": "raw",
							"raw": "{\n    \"title\": \"Coffee\",\n    \"recipe\": [{\n        \"name\": \"Coffee\",\n        \"color\": \"Dark Brown\",\n        \"parts\": 2\n    }]\n}"
						},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks/1",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 401\", function () {",
									"    pm.response.to.have.status(401);",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks/1",
						"method": "PATCH",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": ""
						},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks/1",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 401\", function () {",
									"    pm.response.to.have.status(401);",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks/1",
						"method": "DELETE",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": ""
						},
						"description": ""
					},
					"response": []
				}
			]
		},
		{
			"name": "barista",
			"description": "",
			"item": [
				{
					"name": "/drinks",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 200\", function () {",
									"    pm.response.to.have.status(200);",
									"});",
									"",
									"pm.test(\"value contains drinks array\", function () {",
									"    var jsonData = pm.response.json();",
									"    pm.expect(jsonData.drinks).to.be.an('array')",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks",
						"method": "GET",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": ""
						},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks-detail",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 200\", function () {",
									"    pm.response.to.have.status(200);",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks-detail",
						"method": "GET",
						"header": [
							{
								"key": "Authorization",
								"value": "Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ill1Y0NnYU5XaDh4SWttcnpXUEltRCJ9.eyJpc3MiOiJodHRwczovL215Y29mZmVlYXBpLnVzLmF1dGgwLmNvbS8iLCJzdWIiOiJhdXRoMHw1ZWZhOWUzMzcxNDY4YzAwMTNmZmJiOGIiLCJhdWQiOiJDb2ZmZWUiLCJpYXQiOjE1OTM1NjM0NTYsImV4cCI6MTU5MzU3MDY1NiwiYXpwIjoiTjJJRDZBMmZnWHBKZnBYdTA2WWFnQTBZZ2YwMjBHdTkiLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbImdldDpkcmlua3MtZGV0YWlsIl19.IIHS823LxMpEqQU5r9eqe1WiDvUwyqqJFhXutbWaX2mYjl1GYyJrQAtyuinPA3Qr9Kvera3APv74LiwnY3mHkuUWUYzzjKmdmPD9MO-jDv9TJYJQWW9ok_A0ZZ4hsmSsviexnkpMkfFyJEZGeFsfsa2-DRx_VbI1_lAba0VvT9eosYlRYHKK2c_sCkYUrd4ytc4Iijp3jpGk4NpEmGVF5rqYHpePXih7lgNqMqMf709Kcsnd5UEPCFn4Y6nLmEQpLRqk5bjCaVpgxC2ZvPjNcSQl3RrZOENTxirNw7C35SWN03ROI7w2Ir_ET0NLD67QB1cKFwE_T2mfS3qvNj_5DQ",
								"description": ""
							}
						],
						"body": {},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 401\", function () {",
									"    pm.response.to.have.status(401);",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks",
						"method": "POST",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": ""
						},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks/1",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 401\", function () {",
									"    pm.response.to.have.status(401);",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks/1",
						"method": "PATCH",
						"header": [
							{
								"key": "Authorization",
								"value": "Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ill1Y0NnYU5XaDh4SWttcnpXUEltRCJ9.eyJpc3MiOiJodHRwczovL215Y29mZmVlYXBpLnVzLmF1dGgwLmNvbS8iLCJzdWIiOiJhdXRoMHw1ZWZhOWUzMzcxNDY4YzAwMTNmZmJiOGIiLCJhdWQiOiJDb2ZmZWUiLCJpYXQiOjE1OTM1NjMxNDcsImV4cCI6MTU5MzU3MDM0NywiYXpwIjoiTjJJRDZBMmZnWHBKZnBYdTA2WWFnQTBZZ2YwMjBHdTkiLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbImdldDpkcmlua3MtZGV0YWlsIl19.csEuCHniIFmc4RuXQPz9jDEnVwIpz5SYawdTl2GR-7pxz3AGCB_0FxbudOIBktyWB155tIyvYMoZypCU4OfxxKOmiucDT8BlgsqZLTv0nUbpnpMlyI35zfg6ZNwjZhenxaAMJJcFoSWdN5dIUcaCROGiyhoUMdqzLnF2lm0ao3FSidu1vYrfcOG-ZJWD_q2fz_k4u5WbZt-CGWiORxj2GOMrRn0dD1Es2ZN4ZMeOsyMdw_8IJBTtw6Z9QkJexI_YHtk4sZtS6jMUW0_oTpb9ZBLh7pUtRrM2GLLTpK8knd3h6lxChUY1tfft_ibqaTQTvlueGlJxyprA3SFZUAdXUQ",
								"description": ""
							},
							{
								"key": "Content-Type",
								"value": "application/json",
								"description": ""
							}
						],
						"body": {
							"mode": "raw",
							"raw": "{\n    \"title\": \"Water7\"\n}"
						},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks/1",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 401\", function () {",
									"    pm.response.to.have.status(401);",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks/1",
						"method": "DELETE",
						"header": [
							{
								"key": "Authorization",
								"value": "Bearer",
								"description": ""
							}
						],
						"body": {},
						"description": ""
					},
					"response": []
				}
			]
		},
		{
			"name": "manager",
			"description": "",
			"item": [
				{
					"name": "/drinks",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 200\", function () {",
									"    pm.response.to.have.status(200);",
									"});",
									"",
									"pm.test(\"value contains drinks array\", function () {",
									"    var jsonData = pm.response.json();",
									"    pm.expect(jsonData.drinks).to.be.an('array')",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks",
						"method": "GET",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": ""
						},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks-detail",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 200\", function () {",
									"    pm.response.to.have.status(200);",
									"});",
									"",
									"pm.test(\"value contains drinks array\", function () {",
									"    var jsonData = pm.response.json();",
									"    pm.expect(jsonData.drinks).to.be.an('array')",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks-detail",
						"method": "GET",
						"header": [
							{
								"key": "Authorization",
								"value": "Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ill1Y0NnYU5XaDh4SWttcnpXUEltRCJ9.eyJpc3MiOiJodHRwczovL215Y29mZmVlYXBpLnVzLmF1dGgwLmNvbS8iLCJzdWIiOiJhdXRoMHw1ZWZhOWU2YTJlYjMwMzAwMTljODA5NWUiLCJhdWQiOiJDb2ZmZWUiLCJpYXQiOjE1OTM1NjY5OTcsImV4cCI6MTU5MzU3NDE5NywiYXpwIjoiTjJJRDZBMmZnWHBKZnBYdTA2WWFnQTBZZ2YwMjBHdTkiLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbImRlbGV0ZTpkcmlua3MiLCJnZXQ6ZHJpbmtzLWRldGFpbCIsInBhdGNoOmRyaW5rcyIsInBvc3Q6ZHJpbmtzIl19.q3KPeYP4gVoW5CAEgFxFyiUgzRiYgis29IyVBL5BIuWvmAr8hQMpMSFyiDxylz1jlp82Uhoo39YPJtTQpLxpTCbW1EKZ5Zuad2pe1a7niU-VzjTNEhCFKOj3fwWuojAsHBkIlFuE0h7iH7glULKDCEGndRZ1Q4416MdSIDMeFLnWCCJG8w5VLRE7o0cUENjvuW3q3iE-uwtVDBftV3ZqyzPJkQHkT4s37qnuxvF_X9NUUNFCQhMlh4l2l5YwaIV-0yOdvX8agr4PV-ewfjxHyJ3xCx6HyOo2q1g5TULcQzBax06fDWqjD9XIxIPc_7tuKaQeVoMcqtQ31KL4HdB7pg",
								"description": ""
							}
						],
						"body": {},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 200\", function () {",
									"    pm.response.to.have.status(200);",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks",
						"method": "POST",
						"header": [
							{
								"key": "Content-Type",
								"value": "application/json",
								"description": ""
							},
							{
								"key": "Authorization",
								"value": "Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ill1Y0NnYU5XaDh4SWttcnpXUEltRCJ9.eyJpc3MiOiJodHRwczovL215Y29mZmVlYXBpLnVzLmF1dGgwLmNvbS8iLCJzdWIiOiJhdXRoMHw1ZWZhOWU2YTJlYjMwMzAwMTljODA5NWUiLCJhdWQiOiJDb2ZmZWUiLCJpYXQiOjE1OTM1NjY5OTcsImV4cCI6MTU5MzU3NDE5NywiYXpwIjoiTjJJRDZBMmZnWHBKZnBYdTA2WWFnQTBZZ2YwMjBHdTkiLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbImRlbGV0ZTpkcmlua3MiLCJnZXQ6ZHJpbmtzLWRldGFpbCIsInBhdGNoOmRyaW5rcyIsInBvc3Q6ZHJpbmtzIl19.q3KPeYP4gVoW5CAEgFxFyiUgzRiYgis29IyVBL5BIuWvmAr8hQMpMSFyiDxylz1jlp82Uhoo39YPJtTQpLxpTCbW1EKZ5Zuad2pe1a7niU-VzjTNEhCFKOj3fwWuojAsHBkIlFuE0h7iH7glULKDCEGndRZ1Q4416MdSIDMeFLnWCCJG8w5VLRE7o0cUENjvuW3q3iE-uwtVDBftV3ZqyzPJkQHkT4s37qnuxvF_X9NUUNFCQhMlh4l2l5YwaIV-0yOdvX8agr4PV-ewfjxHyJ3xCx6HyOo2q1g5TULcQzBax06fDWqjD9XIxIPc_7tuKaQeVoMcqtQ31KL4HdB7pg",
								"description": ""
							}
						],
						"body": {
							"mode": "raw",
							"raw": "{\n    \"title\": \"Water\",\n    \"recipe\": {\n        \"name\": \"Water\",\n        \"color\": \"blue\",\n        \"parts\": 1\n    }\n}"
						},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks/1",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 200\", function () {",
									"    pm.response.to.have.status(200);",
									"});",
									"",
									"pm.test(\"value contains drinks array\", function () {",
									"    var jsonData = pm.response.json();",
									"    pm.expect(jsonData.drinks).to.be.an('array')",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks/1",
						"method": "PATCH",
						"header": [
							{
								"key": "Content-Type",
								"value": "application/json",
								"description": ""
							},
							{
								"key": "Authorization",
								"value": "Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ill1Y0NnYU5XaDh4SWttcnpXUEltRCJ9.eyJpc3MiOiJodHRwczovL215Y29mZmVlYXBpLnVzLmF1dGgwLmNvbS8iLCJzdWIiOiJhdXRoMHw1ZWZhOWU2YTJlYjMwMzAwMTljODA5NWUiLCJhdWQiOiJDb2ZmZWUiLCJpYXQiOjE1OTM1NjY5OTcsImV4cCI6MTU5MzU3NDE5NywiYXpwIjoiTjJJRDZBMmZnWHBKZnBYdTA2WWFnQTBZZ2YwMjBHdTkiLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbImRlbGV0ZTpkcmlua3MiLCJnZXQ6ZHJpbmtzLWRldGFpbCIsInBhdGNoOmRyaW5rcyIsInBvc3Q6ZHJpbmtzIl19.q3KPeYP4gVoW5CAEgFxFyiUgzRiYgis29IyVBL5BIuWvmAr8hQMpMSFyiDxylz1jlp82Uhoo39YPJtTQpLxpTCbW1EKZ5Zuad2pe1a7niU-VzjTNEhCFKOj3fwWuojAsHBkIlFuE0h7iH7glULKDCEGndRZ1Q4416MdSIDMeFLnWCCJG8w5VLRE7o0cUENjvuW3q3iE-uwtVDBftV3ZqyzPJkQHkT4s37qnuxvF_X9NUUNFCQhMlh4l2l5YwaIV-0yOdvX8agr4PV-ewfjxHyJ3xCx6HyOo2q1g5TULcQzBax06fDWqjD9XIxIPc_7tuKaQeVoMcqtQ31KL4HdB7pg",
								"description": ""
							}
						],
						"body": {
							"mode": "raw",
							"raw": "{\n    \"title\": \"Water6\"\n}"
						},
						"description": ""
					},
					"response": []
				},
				{
					"name": "/drinks/1",
					"event": [
						{
							"listen": "test",
							"script": {
								"type": "text/javascript",
								"exec": [
									"pm.test(\"Status code is 200\", function () {",
									"    pm.response.to.have.status(200);",
									"});"
								]
							}
						}
					],
					"request": {
						"url": "{{host}}/drinks/1",
						"method": "DELETE",
						"header": [
							{
								"key": "Authorization",
								"value": "Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ill1Y0NnYU5XaDh4SWttcnpXUEltRCJ9.eyJpc3MiOiJodHRwczovL215Y29mZmVlYXBpLnVzLmF1dGgwLmNvbS8iLCJzdWIiOiJhdXRoMHw1ZWZhOWU2YTJlYjMwMzAwMTljODA5NWUiLCJhdWQiOiJDb2ZmZWUiLCJpYXQiOjE1OTM1NjY5OTcsImV4cCI6MTU5MzU3NDE5NywiYXpwIjoiTjJJRDZBMmZnWHBKZnBYdTA2WWFnQTBZZ2YwMjBHdTkiLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbImRlbGV0ZTpkcmlua3MiLCJnZXQ6ZHJpbmtzLWRldGFpbCIsInBhdGNoOmRyaW5rcyIsInBvc3Q6ZHJpbmtzIl19.q3KPeYP4gVoW5CAEgFxFyiUgzRiYgis29IyVBL5BIuWvmAr8hQMpMSFyiDxylz1jlp82Uhoo39YPJtTQpLxpTCbW1EKZ5Zuad2pe1a7niU-VzjTNEhCFKOj3fwWuojAsHBkIlFuE0h7iH7glULKDCEGndRZ1Q4416MdSIDMeFLnWCCJG8w5VLRE7o0cUENjvuW3q3iE-uwtVDBftV3ZqyzPJkQHkT4s37qnuxvF_X9NUUNFCQhMlh4l2l5YwaIV-0yOdvX8agr4PV-ewfjxHyJ3xCx6HyOo2q1g5TULcQzBax06fDWqjD9XIxIPc_7tuKaQeVoMcqtQ31KL4HdB7pg",
								"description": ""
							}
						],
						"body": {},
						"description": ""
					},
					"response": []
				}
			]
		}
	]
}