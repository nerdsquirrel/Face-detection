
## what will be the output of the following code:
```csharp
class Parent
{
    public virtual void Print()
    {
        Console.WriteLine("Parent");
    }
}

class ChildOne : Parent
{
    public new virtual void Print()
    {
        Console.WriteLine("ChildOne");
    }
}

class ChildTwo : ChildOne
{
    public override void Print()
    {
        Console.WriteLine("ChildTwo");
    }
}

static void Main(string[] args)
{
    Parent p = new ChildTwo();
    p.Print();    
    
    ChildOne ch1 = new ChildTwo();
    ch1.Print();
}
```

