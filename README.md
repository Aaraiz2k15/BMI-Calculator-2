# BMI-Calculator-2
BMI calculator built with Python 

def main():
    name = input("what is your name? ").title()

    age = int(input(f"What is your age {name}? "))

    gender = input(f"What is gender {name}? ")

    height  = float(input(f"What is height in cm {name}? "))

    weight = float(input(f"What is weight in kg {name}? "))

    height = height / 100

    bmi = weight / (height * height)

    print(f"Your BMI is: {bmi:.2f}")

    if bmi < 18.5:
        print(f"You are Underweight, {name}!")

    elif bmi < 25:
        print(f"You are in the Healthy Weight range, {name}!")

    elif bmi < 30:
        print(f"You are Overweight, {name}!")

    else:
        print(f"Your BMI is 30 or higher, {name}!")
main()
