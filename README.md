import matplotlib.pyplot as plt

# Define the data
date = input("Enter the date (e.g., 25th June 2020): ")
vaccinated = int(input("Enter the number of vaccinated individuals: ").replace(",", ""))
not_vaccinated = int(input("Enter the number of not vaccinated individuals: ").replace(",", ""))

# Create the pie chart
labels = ['Vaccinated', 'Not Vaccinated']
sizes = [vaccinated, not_vaccinated]
plt.pie(sizes, labels=labels, autopct='%1.1f%%')
plt.title(f'Vaccination Statistics for Germany on {date}')
plt.show()

