Hey everyone! Welcome to this GitHub repository. In this repo, I'll explain how to use Jupyter Notebook on macOS.

I also have a YouTube video that you can find [link to your video]. In the video, I've used this Git repository for easy access for users.

You can copy and paste commands from this repository, or even fork the repo so it will be available in your GitHub account.



# Step 1 

The easiest way to check if Python is installed on your Mac is to open the Terminal application and type the following command

Opening the Terminal on a Mac is straightforward. Here are one way to do it

### 1. Using Spotlight Search

------------
    1 Press Command + Space to open Spotlight Search.
    2 Type Terminal.
    3 Press Enter to open the Terminal application.
------------

```
Terminal
```

```
python -V
```
```Python 3.11.3```

```
python3 -V
```
```Python 3.12.4```



## Create virtual Envirnment in python

[Start creating virtual Envirnment in python ](https://github.com/chaushimran/ichaush_python/blob/main/code/python_venv.md)


# Step 2

## Install python

[Install python](https://github.com/chaushimran/ichaush_python/blob/main/code/Python.md)

# Step 3

[Anaconda](https://github.com/chaushimran/ichaush_python/blob/main/code/anaconda.md)


# Step 4

```
pip install matplotlib
```

```
# Import necessary libraries
import matplotlib.pyplot as plt

# Data for the popularity of programming languages over 10 years
years = [2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023]
languages = ['Python', 'JavaScript', 'Java', 'C#', 'C++']
popularity = {
    'Python': [14, 15, 16, 17, 18, 19, 20, 22, 24, 26],
    'JavaScript': [18, 19, 20, 21, 22, 23, 24, 25, 26, 27],
    'Java': [20, 20, 19, 19, 18, 18, 17, 16, 15, 14],
    'C#': [10, 10, 11, 11, 12, 12, 12, 12, 12, 12],
    'C++': [8, 8, 8, 7, 7, 7, 7, 7, 7, 7]
}

# Create the plot
plt.figure(figsize=(14, 8))

# Plot each language's popularity over time
for language in languages:
    plt.plot(years, popularity[language], marker='o', linestyle='-', label=language)

# Add titles and labels
plt.title('Popularity of Programming Languages Over 10 Years', fontsize=16)
plt.xlabel('Year', fontsize=14)
plt.ylabel('Percentage of Developers Using the Language (%)', fontsize=14)

# Adding a legend
plt.legend(loc='upper left', fontsize=12)

# Customizing the grid
plt.grid(color='gray', linestyle='--', linewidth=0.5)

# Adding annotations for the last point of each language
for language in languages:
    plt.annotate(f'{popularity[language][-1]}%', 
                 (years[-1], popularity[language][-1]), 
                 textcoords="offset points", 
                 xytext=(0,10), 
                 ha='center')

# Display the plot
plt.show()
```
