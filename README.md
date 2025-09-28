# Using-Faker-Module
For extra credit, I chose the faker module because it’s simple but very practical. It lets you generate realistic-looking fake data (names, emails, addresses, etc.), which is especially helpful when you need to test programs without using sensitive information.

Faker Demo

This repository shows how to use the `faker` module to generate fake data
for testing and practice.

Installation
------------

`faker` is not part of the standard library. Install it with:

   pip install faker


Example
-------

from faker import Faker

def generate_fake_data(records=5):
    fake = Faker()
    for _ in range(records):
        print("Name:", fake.name())
        print("Email:", fake.email())
        print("Address:", fake.address())
        print("-" * 40)
print (generate_fake_data(5))

This would then generate 5 different non-existent people.

Expected Output 

Name: Jacob Garcia
Email: opeck@example.org
Address: 4607 Baker Plaza Apt. 436
Allenland, OH 13128
----------------------------------------
Name: Heidi Jones
Email: nicolegoodman@example.com
Address: 8221 Rivera Village Suite 804
New Sarahland, IN 58527
----------------------------------------
Name: Mr. David Davis
Email: hgarcia@example.com
Address: PSC 3854, Box 1554
APO AE 74705
----------------------------------------
Name: Michael Hill
Email: michael73@example.com
Address: 5877 Evans Stravenue
Olsenfort, AL 04836
----------------------------------------
Name: David Cross
Email: andrewclay@example.com
Address: 4919 Austin Hollow
South Jenniferport, ME 83785
----------------------------------------
None
