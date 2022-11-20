# qb-policejob w/ Multi-department
[QB-Policejob] Multi-department


This version of qb-policejob supports multiple police departments by changing playerjob.name = 'police' to playerjob.type = 'leo'

Below is an example of how to add policejob to qb-core / shared / jobs.lua to make them work with the police job. As you can see in the example below type = "leo".

```
['bcso'] = {
	label = 'Blaine County Sheriff Dept',
        type = "leo",
	defaultDuty = true,
	offDutyPay = false,
	grades = {
        	['0'] = { name = 'Recruit', payment = 200 },
		['1'] = { name = 'Deputy', payment = 250 },
		['2'] = { name = 'Senior Deputy', payment = 275 },
		['3'] = { name = 'Corporal', payment = 300 },
		['4'] = { name = 'Sergeant', payment = 350 },
        	['5'] = { name = 'Lieutenant', payment = 375 },
        	['6'] = { name = 'Captain', payment = 400 },
        	['7'] = { name = 'Deputy Sheriff', payment = 450 },
        	['8'] = { name = 'Sheriff', isboss = true, bankAuth = true, payment = 500 },
        },
},
  ```
