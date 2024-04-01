#include <iostream>

class Mechanic
{
public:
    virtual void go()
    {
        std::cout << "Ты идешь\n";
    }
};

class Swim : public Mechanic
{
public: 
    void go() override
    {
        std::cout << "Ты плаваешь\n";
    }
};

class Fly : public Mechanic
{
public:
    void go() override
    {
        std::cout << "Ты летишь\n";
    }
};

class Climb : public Mechanic
{
public:
    void go() override
    {
        std::cout << "Ты карабкаешься\n";
    }
};

class Teleportation : public Mechanic
{
public:
    void go() override
    {
        std::cout << "Ты телепортировался\n";
    }
};

class Person
{
public: 
    void go(Mechanic* mechanic)
    {
        mechanic->go();
    }
};

int main()
{
    setlocale(0, "");
    Person person;

    Swim swim;
    Fly fly;
    Climb climb;
    Teleportation teleportation;

    person.go(&swim);
    person.go(&fly);
    person.go(&climb);
    person.go(&teleportation);
}
