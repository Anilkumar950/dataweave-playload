# dataweave-playload

{
	"students": [{
			"name": "Ramesh",
			"email": "ramesh@gmail.com",
			"yearofbirth": 1996,
			"school": "M.M High school",
			"Marks_2020": [{
				"Jan": 500,
				"Feb": 500,
				"Mar": 500
			}]
		},
		{
			"name": "Manish",
			"email": "Manish12@gmail.com",
			"yearofbirth": 1992,
			"school": "st pauls ",
			"Marks_2020": [{
				"Jan": 400,
				"Feb": 400,
				"Mar": 400
			}]
		},
		{
			"name": "srikanth",
			"email": "srikanth@gmail.com",
			"yearofbirth": 2000,
			"school": "st pauls",
			"Marks_2020": [{
				"Jan": 600,
				"Feb": 600,
				"Mar": 600
			}]
		},
		{
			"name": "kishor",
			"email": "kishor@gmail.com",
			"yearofbirth": 1992,
			"school": "M.M High school",
			"Marks_2020": [{
				"Jan": 500,
				"Feb": 500,
				"Mar": 500
			}]
		},
		{
			"name": "Vani",
			"email": "vani@gmail.com",
			"yearofbirth": 1993,
			"school": "st pauls",
			"Marks_2020": [{
				"Jan": 700,
				"Feb": 700,
				"Mar": 700
			}]
		},
		{
			"name": "ram",
			"email": "ram@gmail.com",
			"yearofbirth": 1995,
			"school": "M.M High school",
			"Marks_2020": [{
				"Jan": 800,
				"Feb": 800,
				"Mar": 800
			}]
		}
	]
}

condition0: payload.students -------------->(printing the full information)
condition1: payload.students.name  ------------>(only names printing)
condition2: (payload.students) orderBy($.yearofbirth) --------------->(printing the orderBy ex: 1,2,3,4,5,6)
condition3: payload.students[1]  -------------------->(only one student information)

