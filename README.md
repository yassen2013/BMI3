# BMI3
def calulate_bmi(weight, height):
    """Calculate the Body Mass Index (BMI)."""
    return weight / (height**2)



def classif_bmi(bmi):
    """Classif the BMI value based on its range."""

    if bmi < 16:
        return "Severe Thinness"
    elif 16 <=bmi <16.9:
        return "Moderate Thinness"
    elif 17 <=bmi <18.9:
        return "Mild Thiness"
    elif 18.5 <=bmi <24.9:
        return "Normal weight"
    elif 25 <=bmi <29.9:
        return "Overweight"
    elif 30 <= bmi < 34.9:
        return "Obesity Class 1"
    elif 35 <= bmi < 39.9:
        return "Obesity Class 2"
    else:
        return "Obesity Class 3(Severe Obesity)"
def main():
        weight = float(input("Enter weight in Killograms"))
        height = float(input("Enter height in meters:"))
        bmi = calulate_bmi((weight, height))
        print(f"BMI is: {bmi:.2f}")
        print(f"Classification:{calulate_bmi(bmi)}")

if _name_ == "_main_":
    main()
