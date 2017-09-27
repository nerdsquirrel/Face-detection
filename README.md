
## what will be the output of the following code:
```csharp
static void Main(sting[] args)
{
	var emplist = new List<Employee>(
		new Employee[]
		{
			new Employee{Id =1, Name = "Jack", Age = 32},
			new Employee{Id =2, Name = "Rahul", Age = 30},
			new Employee{Id =3, Name = "Sheela", Age = 23},
			new Employee{Id =4, Name = "Mary", Age = 25}
		});	
		
	var lst = from e in emplist where e.Age>25 select new {e.Name};

	emplist.Add(new Employee{Id =5, Name = "Bill", Age = 38});
	
	foreach(var emp in lst)
		Console.WriteLine(emp.Name);
}
```

