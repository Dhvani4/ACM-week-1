{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/Dhvani4/ACM-week-1/blob/main/README.md\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "# **ACM Task 1**\n",
        "\n",
        "Welcome mentees to your first task in ACM!\n",
        "\n",
        "\n",
        "Our focus this week is on mastering [Python](http://alturl.com/5536k)—a language that powers countless applications, from web development to AI and data science. By the end of this notebook, you’ll have a strong foundation in Python that will serve as a stepping stone for more advanced topics in the coming weeks.\n",
        "\n",
        "Whether you’re new to Python or looking to solidify your understanding, this task will set the stage for everything we’ll cover throughout the learning period.\n",
        "\n",
        "Please don’t hesitate to reach out with any questions. We’re here to support you every step of the way.\n",
        "\n",
        "Let’s dive in and start coding!"
      ],
      "metadata": {
        "id": "bugnHkGyHHj5"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## **NOTE:**\n",
        "\n",
        "**Copy this notebook to your own drive (click on 'File' option in the NavBar' and select 'Save a copy in Drive') and then run the notebook and make whatever changes you want on it. Once you have finished the task, push the notebook to a GitHub repository named 'ACM\\_24_task\\_1'.**"
      ],
      "metadata": {
        "id": "2hsWkr1yGqmH"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Colab Notebook Execution"
      ],
      "metadata": {
        "id": "XY4yMkngKWv6"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "We will use Jupyter notebooks and Google colab as the primary way to practice machine learning. Notebooks are a great way to mix executable code with rich contents (HTML, images, equations written in LaTeX). Colab allows to run notebooks on the cloud for free without any prior installation, while leveraging the power of [GPUs](https://en.wikipedia.org/wiki/Graphics_processing_unit)."
      ],
      "metadata": {
        "id": "fLk-YXApKGD7"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "The document that you are reading is not a static web page, but an interactive environment called a notebook, that lets you write and execute code. Notebooks consist of so-called code cells, blocks of one or more Python instructions. For example, here is a code cell that stores the result of a computation (the number of seconds in a day) in a variable and prints its value:"
      ],
      "metadata": {
        "id": "3WU0qHuqKQXQ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "seconds_in_a_day = 24 * 60 * 60\n",
        "seconds_in_a_day\n",
        "multiply=28*4\n",
        "multiply"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "YMkzXOXyKU_o",
        "outputId": "9ea79a76-a737-49d4-89ba-0e91c7dce3e3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "112"
            ]
          },
          "metadata": {},
          "execution_count": 1
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "multiply=2*4*5\n",
        "multiply"
      ],
      "metadata": {
        "id": "1B8xIh7AhVBH",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "5cca6077-8fe6-4129-fc01-2a0096bcf1b9"
      },
      "execution_count": 1,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "40"
            ]
          },
          "metadata": {},
          "execution_count": 1
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Click on the \"play\" button to execute the cell. You should be able to see the result. Alternatively, you can also execute the cell by pressing Ctrl + Enter if you are on Windows / Linux or Command + Enter if you are on a Mac."
      ],
      "metadata": {
        "id": "SJ1jX0XiKfk6"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## I/O"
      ],
      "metadata": {
        "id": "aURtzRhqI9au"
      }
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "8k_e19mRFcsk",
        "outputId": "20e5f74d-7aa5-4d6a-de6e-a10dd75b3cb4"
      },
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What is your name? dhvani\n",
            "Hello, dhvani\n",
            "what is your birthplace mumbai\n",
            "mumbai\n"
          ]
        }
      ],
      "source": [
        "name = input(\"What is your name? \") # String input\n",
        "print(\"Hello,\", name)\n",
        "birthplace=input(\"what is your birthplace \")\n",
        "print(birthplace)"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "dob = int(input(\"When were you born? \")) # Integer input (try removing the int() function and see what happens!)\n",
        "print(\"You are\", 2024 - dob, \"years old.\") # Like integer, you can do above for other data types like float as well"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "WAfUg1_5JLjL",
        "outputId": "6da1ef50-7cf9-4fcf-a342-ad788a311cc3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "When were you born? 2005\n",
            "You are 19 years old.\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "## Different ways to print\n",
        "age = 2024 - dob\n",
        "print(\"You are\", age, \"years old.\") # Simplest way to print\n",
        "print(\"You are \" + str(age) + \" years old.\") # Via String Concatenation\n",
        "print(f\"You are {age} years old.\") # Via f-strings (introduced in python 3.6)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "YfjihY8jJVvX",
        "outputId": "90c44088-a8ad-4785-a69a-0af652b22ad7"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "You are 19 years old.\n",
            "You are 19 years old.\n",
            "You are 19 years old.\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(\"I am a ACM Mentee.\", end=\" \") # Change print output from newline to single space.\n",
        "print(\"I am a DJ Sanghvi student.\")\n",
        "print(\"Hello\",end=\" \")\n",
        "print(\"My name is Dhvani\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "rX9WPxH4NaXA",
        "outputId": "44396f18-2875-47b6-85a4-cec2212350e6"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "I am a ACM Mentee. I am a DJ Sanghvi student.\n",
            "Hello My name is Dhvani\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "**Exercise Time**\n",
        "\n",
        "- Ask the user to enter their first name.\n",
        "- Store the input in a variable named first_name.\n",
        "- Print a greeting message using the first_name variable.\n",
        "- Experiment with different ways to format the output:\n",
        "  - Using f-strings\n",
        "  - Using the format() method\n",
        "  - Using the % operator"
      ],
      "metadata": {
        "id": "b0zUMF2T75_F"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# write your code here\n",
        "first_name=input(\"what is ur name\")\n",
        "print(\"hello\",first_name)\n",
        "print(f\"hello {first_name}\")\n",
        "print(\"hello, {}\".format(first_name))\n",
        "print(\"Hello, %s\" % first_name)"
      ],
      "metadata": {
        "id": "ECZrVnJ59lU7",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "9b81bdb1-6bd6-4018-e720-e5d2bcd19e4c"
      },
      "execution_count": 2,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "what is ur nameDhvani\n",
            "hello Dhvani\n",
            "hello Dhvani\n",
            "hello, Dhvani\n",
            "Hello, Dhvani\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Expressions and Data Types"
      ],
      "metadata": {
        "id": "3gdWYiPPLBk9"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Python offers a rich set of data types including numbers, strings, lists, dictionaries, and more, each serving specific data handling needs. As a dynamic language, Python determines the data type of a variable at runtime, providing flexibility in assigning different data types to the same variable without explicit declaration.\n",
        "So no need of writing data types of each and every variable. Python is smart enough to figure out on it's own! You can find the type of variables via the type() function. Some common data types you will mostly use are:\n",
        "\n",
        "* Numbers\n",
        "  * integers\n",
        "  * floating-point\n",
        "  * complex numbers\n",
        "* strings\n",
        "* boolean values\n",
        "* lists and dicts"
      ],
      "metadata": {
        "id": "LLRf2ADVLPeB"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "12 + 3.5 # addition"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "5_iXm6qxLQQU",
        "outputId": "6342d95a-18c3-4cd5-dac5-c182fa71d9eb"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "15.5"
            ]
          },
          "metadata": {},
          "execution_count": 7
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "5 - 9.1 # subtraction"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "61mDjvu3LZ3o",
        "outputId": "52f141fd-f5a0-4009-91ee-ab11a26adad8"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "-4.1"
            ]
          },
          "metadata": {},
          "execution_count": 8
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "3.1 * 4 # multiplication"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "dIBpNK-dLd6O",
        "outputId": "73e09d1d-d9ef-477c-caf3-317fb6e53ed5"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "12.4"
            ]
          },
          "metadata": {},
          "execution_count": 9
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "13 / 3 # division"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "19Wyx0G1LiQY",
        "outputId": "6200ad42-5d52-4e59-82b7-16945effac97"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "4.333333333333333"
            ]
          },
          "metadata": {},
          "execution_count": 10
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "round(13 / 3, 2) # rounding off"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "CDZEqq_eO9yk",
        "outputId": "a1934396-d142-4343-807e-6567fdbae1b9"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "4.33"
            ]
          },
          "metadata": {},
          "execution_count": 11
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "2.5 ** 2 # exponentiation"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "LGSCdVDeLlcy",
        "outputId": "de727652-6d63-446d-f8d7-96c588b88615"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "6.25"
            ]
          },
          "metadata": {},
          "execution_count": 12
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "5 + 3j # complex number"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "DtkDL0zyM-0E",
        "outputId": "207d3aa8-6608-4bca-b7fe-1ff53a00d89c"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "(5+3j)"
            ]
          },
          "metadata": {},
          "execution_count": 13
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Conditionals"
      ],
      "metadata": {
        "id": "aZRdsLCmPOeQ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "## if-else statements (note that we use elif instead of else if)\n",
        "score = int(input(\"Score: \"))\n",
        "\n",
        "if 90 <= score <= 100:\n",
        "    print(\"Grade: A\")\n",
        "elif 80 <= score < 90:\n",
        "    print(\"Grade: B\")\n",
        "elif 70 <= score < 80:\n",
        "    print(\"Grade: C\")\n",
        "elif 60 <= score < 70:\n",
        "    print(\"Grade: D\")\n",
        "else:\n",
        "    print(\"Grade: F\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "W5ae1vlyPQuN",
        "outputId": "44d9e271-4c55-4b74-d1e7-eca2a8db9c66"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Score: 65\n",
            "Grade: D\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "In the programming world, there are types of programming that are called “Pythonic” in nature. That is, there are ways to program that are sometimes only seen in Python programming. Notice that this statement in our code is almost like a sentence in English. This is a unique way of coding only seen in Python."
      ],
      "metadata": {
        "id": "dXDEHf7ZQcw6"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "print(\"You are eligible to vote\" if dob <= 2006 else \"You are not eligible to vote\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "B3xeHzCkQEBw",
        "outputId": "cddc1bb1-60bd-48eb-a091-0ddeca4db23b"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "You are eligible to vote\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "# Instead of switch, we use match in python. (Note how instead of default, we have used case _)\n",
        "name = input(\"What's your name? \")\n",
        "\n",
        "match name:\n",
        "    case \"Harry\":\n",
        "        print(\"Gryffindor\")\n",
        "    case \"Hermione\":\n",
        "        print(\"Gryffindor\")\n",
        "    case \"Ron\":\n",
        "        print(\"Gryffindor\")\n",
        "    case \"Draco\":\n",
        "        print(\"Slytherin\")\n",
        "    case _:\n",
        "        print(\"Who?\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "GBvnb76VQyvB",
        "outputId": "8f1c65ed-308e-4a88-da81-d4e109ed8aef"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What's your name? Draco\n",
            "Slytherin\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "There is some redundancy in the above code. See how I have [refactored](https://www.agilealliance.org/glossary/refactoring/) the code:"
      ],
      "metadata": {
        "id": "qa9p25gNRa6F"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "name = input(\"What's your name? \")\n",
        "\n",
        "match name:\n",
        "    case \"Harry\" | \"Hermione\" | \"Ron\":\n",
        "        print(\"Gryffindor\")\n",
        "    case \"Draco\":\n",
        "        print(\"Slytherin\")\n",
        "    case _:\n",
        "        print(\"Who?\")\n",
        "\n",
        "# Notice, the use of the single vertical bar |. This allows us to check for multiple values in the same case statement."
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "OclOLSbHRCi6",
        "outputId": "fc97e14a-a8f7-41f9-c113-755a87e1d125"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What's your name? Hermione\n",
            "Gryffindor\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "**Exercise Time**\n",
        "\n",
        "Scenario:\n",
        "You are a budding potioneer at Hogwarts. You need to create a potion of a specific strength. The strength of a potion is determined by the ratio of its ingredients.\n",
        "\n",
        "Instructions:\n",
        "\n",
        "Gather ingredients:\n",
        "\n",
        "- Ask the user to input the quantity of two ingredients (e.g., Snape's Special Spice and Newt's Nodule Extract).\n",
        "- Store these values as numerical variables.\n",
        "\n",
        "Calculate potion strength:\n",
        "\n",
        "The potion strength is calculated as the ratio of Snape's Special Spice to the total quantity of both ingredients.\n",
        "Calculate and store the potion strength as a percentage.\n",
        "Determine potion quality:\n",
        "\n",
        "- If the potion strength is between 30% and 70%, print \"Acceptable Potion\".\n",
        "- If the potion strength is less than 30%, print \"Potion is too weak!\".\n",
        "- If the potion strength is greater than 70%, print \"Potion is too strong!\"."
      ],
      "metadata": {
        "id": "tqUhvc2WIkdJ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# write your code here\n",
        "q1=int(input(\"enter the quantity of snape`s special spice\"))\n",
        "q2=int(input(\"enter the quantity of newt`s nodule extract\"))\n",
        "strength=(q1/(q1+q2))*100\n",
        "if 70 >= strength >= 30 :\n",
        "    print(\"Acceptable potion\")\n",
        "elif 30 > strength :\n",
        "    print(\"Potion is too weak\")\n",
        "elif 70< strength:\n",
        "    print(\"Potion is too strong\")"
      ],
      "metadata": {
        "id": "OnbpQWQWIhN5",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "c863920a-e229-4c59-c37a-e9b3af25cea0"
      },
      "execution_count": 3,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "enter the quantity of snape`s special spice70\n",
            "enter the quantity of newt`s nodule extract70\n",
            "Acceptable potion\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Loops"
      ],
      "metadata": {
        "id": "gBkfsuefSZzf"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# while loop remains the same as always\n",
        "i = 3\n",
        "while i != 0:\n",
        "  print(\"meow\")\n",
        "  i = i - 1"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "ehePei0eSbRr",
        "outputId": "7a3f4e80-35d9-475c-9498-9e0239575279"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "meow\n",
            "meow\n",
            "meow\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "There is a major change in how we write for loops. To best understand a for loop, it’s best to begin by talking about a new variable type called a list in Python. As in other areas of our lives, we can have a grocery list, a to-do list, etc. A for loop iterates through a list of items."
      ],
      "metadata": {
        "id": "Sc-qvLHRSwkt"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "for i in [0, 1, 2]: # here [0, 1, 2] is a list (similar to arrays)\n",
        "    print(\"meow\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Ptn9cDVnS6Y9",
        "outputId": "94b387fa-7be3-4383-a4fc-c55700e54b42"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "meow\n",
            "meow\n",
            "meow\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "However, what if you wanted to iterate up to a million? It’s best to create code that can work with such extreme cases."
      ],
      "metadata": {
        "id": "kMNAw7vFTOVf"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "for i in range(3):\n",
        "    print(i, end=\", \") # note how execution starts from 0"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "ObxQIF37TNlx",
        "outputId": "bdd19a3b-3dc2-428b-eab7-d5db1ad074c1"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0, 1, 2, "
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "What if I want to print numbers from 5 to 11 skipping even numbers? Consider the below code:"
      ],
      "metadata": {
        "id": "DkVZR9sPVUgY"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "for i in range(5, 12, 2):\n",
        "    print(i, end=\", \")\n",
        "\n",
        "# The first parameter is the initial value, second is when the loop should stop (it will stop one number before it)\n",
        "# and the third is how should the variable be incremented/decremented/changed (this is skippable, python will default to 1)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "5Alfdb_SVT9g",
        "outputId": "656acaef-6db0-4bed-9a29-53def9531ca8"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "5, 7, 9, 11, "
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "In Python, if a variable does not have any other significance in our code, we can simply represent this variable as a single underscore _."
      ],
      "metadata": {
        "id": "L9ZUnsPcUc5e"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "for _ in range(3):\n",
        "    print(\"meow\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Hsei-YmsUcLC",
        "outputId": "ec7f9b27-14c7-4a4a-e35b-57af2c2f54d3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "meow\n",
            "meow\n",
            "meow\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "To stretch your mind to the possibilities within Python, consider the following code:"
      ],
      "metadata": {
        "id": "649L4MqlUv_0"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "print(\"meow\" * 3)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "jzSF6sLDUiYv",
        "outputId": "114a1675-629d-461e-e184-ef1e7fba9073"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "meowmeowmeow\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "**Excerise Time**\n",
        "\n",
        "Notice how the above code will meow three times, but the program will produce meowmeowmeow as the result. Consider: How could you create a line break at the end of each meow?"
      ],
      "metadata": {
        "id": "UnqmDD9SUtwZ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# write your code here\n",
        "print(\"meow\\n\"*3)"
      ],
      "metadata": {
        "id": "Pt_F6fPVVAMq",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "3624908a-4ece-4548-bd9c-b4368cd329e2"
      },
      "execution_count": 4,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "meow\n",
            "meow\n",
            "meow\n",
            "\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Lists"
      ],
      "metadata": {
        "id": "Kw2qoGjoXyHJ"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "You might wonder why we did not use the _ designation as discussed prior. We choose not to do this because student is explicitly used in our code. You can learn more in Python’s documentation of [lists](https://docs.python.org/3/tutorial/datastructures.html#more-on-lists)."
      ],
      "metadata": {
        "id": "aVNVVPFIY7OW"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "students = [\"Hermoine\", \"Harry\", \"Ron\"]\n",
        "\n",
        "for student in students:\n",
        "    print(student)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "THLFCSx9X27H",
        "outputId": "55f5eeb1-e330-4fa2-957e-89aa5a75712d"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Hermoine\n",
            "Harry\n",
            "Ron\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice how executing this code results in not only getting the position of each student plus one using i + 1, but also prints the name of each student. len allows you to dynamically see how long the list of the students is regardless of how much it grows."
      ],
      "metadata": {
        "id": "2hqHVMX_Y2YK"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "students = [\"Hermoine\", \"Harry\", \"Ron\"]\n",
        "\n",
        "for i in range(len(students)):\n",
        "    print(i + 1, students[i])"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "D_4Bvos4YU_C",
        "outputId": "39a8c776-0552-4065-f278-bfff9d672474"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "1 Hermoine\n",
            "2 Harry\n",
            "3 Ron\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "# Some inbuilt list functions:\n",
        "\n",
        "my_list = [1, 2, 3]\n",
        "my_list.append(4) # adds 4 to the end of the list\n",
        "print(my_list)\n",
        "print(my_list[1:3]) # prints the second and third element of the list\n",
        "print(my_list[1:]) # prints the second element to the end of the list\n",
        "print(5 in my_list) # checks if 5 is in the list"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "4ZYTNrWKZJLN",
        "outputId": "e6c3c7cc-382e-4ddb-b07f-e5266c49ae4d"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1, 2, 3, 4]\n",
            "[2, 3]\n",
            "[2, 3, 4]\n",
            "False\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "\"List comprehension\" is the idea of writing some code inside of a list that will generate a list."
      ],
      "metadata": {
        "id": "9x9N1qrxnuDa"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "[x ** 2 for x in range(10)]"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "MNX_1dBenut-",
        "outputId": "729fef66-a72f-45f9-cbe5-b1da4a51c9e4"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"
            ]
          },
          "metadata": {},
          "execution_count": 29
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "**Exercise Time**\n",
        "\n",
        "- Prepare a list of questions related to personality traits, values, and preferences.\n",
        "- Each question should have multiple answer options.\n",
        "- Example questions:\n",
        "  - What kind of course would you be best in? (Charms, Herbology, Defense Against the Dark Arts, Potions)\n",
        "  - Which animal do you instinctively trust? (Dog, Cat, Owl, Horse)\n",
        "  - Which house spirit would be your friend? (Dobby, Kreacher, Pixies)\n",
        "\n",
        "- Present each question to the user and allow them to input their answer.\n",
        "- Store the answers in a list.\n",
        "- Assign points to each answer based on how it aligns with the characteristics of each Hogwarts house (Gryffindor, Hufflepuff, Ravenclaw, Slytherin).\n",
        "- Calculate the total points for each house.\n",
        "- Find the house with the highest point total.\n",
        "- Print the user's assigned Hogwarts house."
      ],
      "metadata": {
        "id": "wasPBk3gI11l"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# write your code here\n",
        "questions = [\"What kind of course would you be best in?\\n1. Charms\\n2. Herbology\\n3. Defense Against the Dark Arts\\n4. Potions\\n\",\"Which animal do you instinctively trust?\\n1. Dog\\n2. Cat\\n3. Owl\\n4. Horse\\n\",\"Which house spirit would be your friend?\\n1. Dobby\\n2. Kreacher\\n3. Pixies\\n\"]\n",
        "answers = []\n",
        "Gryffindor=0\n",
        "Hufflepuff=0\n",
        "Ravenclaw=0\n",
        "Slytherin=0\n",
        "for question in questions:\n",
        "  choice=input(question)\n",
        "  answers.append(choice)\n",
        "print(answers)\n",
        "if answers[0]==\"Charms\":\n",
        "  Gryffindor = Gryffindor+1\n",
        "  Slytherin = Slytherin+2\n",
        "elif answers[0]==\"Herbology\":\n",
        "  Hufflepuff = Hufflepuff+1\n",
        "  Ravenclaw = Ravenclaw+2\n",
        "elif answers[0]==\"Defense Against the Dark Arts\":\n",
        "  Ravenclaw = Ravenclaw+1\n",
        "  Gryffindor = Gryffindor+2\n",
        "elif answers[0]==\"Potions\":\n",
        "  Hufflepuff = Huffleppuff+1\n",
        "\n",
        "else:\n",
        "  print(\"Answer from the choices given\")\n",
        "\n",
        "if answers[1]==\"Dog\":\n",
        "  Gryffindor = Gryffindor+1\n",
        "  Ravenclaw = Ravenclaw+2\n",
        "elif answers[1]==\"Cat\":\n",
        "  Hufflepuff = Hufflepuff+1\n",
        "  Slytherin = Slytherin+2\n",
        "elif answers[1]==\"Owl\":\n",
        "  Ravenclaw = Ravenclaw+1\n",
        "  Gryffindor = Gryffindor+2\n",
        "elif answers[1]==\"Horse\":\n",
        "  Slytherin = Slytherin+1\n",
        "  Hufflepuff = Hufflepuff+2\n",
        "else:\n",
        "  print(\"Answer from the choices given\")\n",
        "\n",
        "if answers[2]==\"Dobby\":\n",
        "  Gryffindor = Gryffindor+1\n",
        "  Ravenclaw=Ravenclaw+2\n",
        "elif answers[2]==\"Kreacher\":\n",
        "  Hufflepuff = Hufflepuff+1\n",
        "elif answers[2]==\"Pixies\":\n",
        "  Ravenclaw = Ravenclaw+1\n",
        "  Slytherin = Slytherin+2\n",
        "else:\n",
        "  print(\"Answer from the choices given\")\n",
        "\n",
        "print(Gryffindor,Hufflepuff,Ravenclaw,Slytherin)\n",
        "print(\"You are assigned to \"+str(max(Gryffindor,Hufflepuff,Ravenclaw,Slytherin)))\n"
      ],
      "metadata": {
        "id": "DfJBNeeGJViI",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "ca247d8a-71be-41b6-e91a-4915eba53458"
      },
      "execution_count": 8,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What kind of course would you be best in?\n",
            "1. Charms\n",
            "2. Herbology\n",
            "3. Defense Against the Dark Arts\n",
            "4. Potions\n",
            "Charms\n",
            "Which animal do you instinctively trust?\n",
            "1. Dog\n",
            "2. Cat\n",
            "3. Owl\n",
            "4. Horse\n",
            "Horse\n",
            "Which house spirit would be your friend?\n",
            "1. Dobby\n",
            "2. Kreacher\n",
            "3. Pixies\n",
            "Dobby\n",
            "['Charms', 'Horse', 'Dobby']\n",
            "2 2 2 3\n",
            "You are assigned to 3\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Dictionaries"
      ],
      "metadata": {
        "id": "zOT357PWZxVy"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "dicts or dictionaries is a data structure that allows you to associate keys with values.\n",
        "Where a list is a list of multiple values, a dict associates a key with a value."
      ],
      "metadata": {
        "id": "j03rXyabZ2hF"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "students = {\n",
        "    \"Hermoine\": \"Gryffindor\",\n",
        "    \"Harry\": \"Gryffindor\",\n",
        "    \"Ron\": \"Gryffindor\",\n",
        "    \"Draco\": \"Slytherin\",\n",
        "}\n",
        "print(students[\"Hermoine\"])\n",
        "print(students[\"Harry\"])\n",
        "print(students[\"Ron\"])\n",
        "print(students[\"Draco\"])"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "EqytEo4uZMUz",
        "outputId": "50d458b8-bf39-4947-8ca5-d713e227041b"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Gryffindor\n",
            "Gryffindor\n",
            "Gryffindor\n",
            "Slytherin\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice how we use {} curly braces to create a dictionary. Where lists use numbers to iterate through the list, dicts allow us to use words."
      ],
      "metadata": {
        "id": "RHX7U3hKaHe-"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "for student in students:\n",
        "    print(student)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "yORG7VNzZ7bt",
        "outputId": "36c0f9e4-28ae-49f0-c851-05cca5234855"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Hermoine\n",
            "Harry\n",
            "Ron\n",
            "Draco\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice how, executing this code, the for loop will only iterate through all the keys, resulting in a list of the names of the students. How could we print out both values and keys?"
      ],
      "metadata": {
        "id": "NEOTjV9QaM8F"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "for student in students:\n",
        "    print(student, students[student], sep=\", \") # sep allows us to alter how different components of a print statement is displayed"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "SiYROj6ZaPUm",
        "outputId": "22891b6e-74ff-46ba-f10c-c49b3071754d"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Hermoine, Gryffindor\n",
            "Harry, Gryffindor\n",
            "Ron, Gryffindor\n",
            "Draco, Slytherin\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "You can imagine wanting to have lots of data associated with multiple keys."
      ],
      "metadata": {
        "id": "01WVplY0arpa"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "students = [\n",
        "    {\"name\": \"Hermoine\", \"house\": \"Gryffindor\", \"patronus\": \"Otter\"},\n",
        "    {\"name\": \"Harry\", \"house\": \"Gryffindor\", \"patronus\": \"Stag\"},\n",
        "    {\"name\": \"Ron\", \"house\": \"Gryffindor\", \"patronus\": \"Jack Russell terrier\"},\n",
        "    {\"name\": \"Draco\", \"house\": \"Slytherin\", \"patronus\": None},\n",
        "]"
      ],
      "metadata": {
        "id": "FE36OkLSarEy"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice how the for loop will iterate through each of the dicts inside the list called students.\n",
        "\n",
        "You can learn more in Python’s Documentation of [dicts](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)."
      ],
      "metadata": {
        "id": "dY5WEKBJa0CZ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "for student in students:\n",
        "    print(student[\"name\"], student[\"house\"], student[\"patronus\"], sep=\", \")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "nk_KE-CBav1v",
        "outputId": "6e021d4d-afcb-4bec-e0ec-83e31e1bf8c4"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Hermoine, Gryffindor, Otter\n",
            "Harry, Gryffindor, Stag\n",
            "Ron, Gryffindor, Jack Russell terrier\n",
            "Draco, Slytherin, None\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "What if I want to access only the keys or only the values of the dictionary? We can do the following."
      ],
      "metadata": {
        "id": "9HtjTO7sbLNw"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "print(\"Keys: \")\n",
        "for i in students[0].keys():\n",
        "    print(f\"\\t{i}\")\n",
        "print(\"Values: \")\n",
        "for i in students[0].values():\n",
        "    print(f\"\\t{i}\")\n",
        "print(\"Items: \")\n",
        "for i in students[0].items():\n",
        "    print(f\"\\t{i}\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "6xYfGgqKbJfx",
        "outputId": "ecde3745-0b47-4485-a211-e7e5e2196c8b"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Keys: \n",
            "\tname\n",
            "\thouse\n",
            "\tpatronus\n",
            "Values: \n",
            "\tHermoine\n",
            "\tGryffindor\n",
            "\tOtter\n",
            "Items: \n",
            "\t('name', 'Hermoine')\n",
            "\t('house', 'Gryffindor')\n",
            "\t('patronus', 'Otter')\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "**Exercise Time**\n",
        "- Create a dictionary to represent a Harry Potter character's inventory.\n",
        "- Use item names as keys and quantities as values. (Such as: \"Gold Galleons\": 100, \"Silver Sickles\": 500, \"Bronze Knuts\": 2000, \"Potion Bottles\": 5).\n",
        "- Allow the user to add or remove items from the inventory.\n",
        "- Update the quantity accordingly.\n",
        "- Assign values to each type of currency (e.g., 1 Galleon = 29 Sickles, 1 Sickle = 29 Knuts).\n",
        "- Calculate the total worth of the inventory in Galleons.\n",
        "- Print the contents of the inventory in a formatted manner."
      ],
      "metadata": {
        "id": "o08LB_nRJy_d"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# write your code here\n",
        "Inventory = [\n",
        "    {\"name\":\"Gold Galleons\",\"quantity\":100},\n",
        "    {\"name\":\"Silver Sickles\",\"quantity\":500},\n",
        "    {\"name\":\"Bronze Knuts\",\"quantity\":2000},\n",
        "    {\"name\":\"Potion Bottles\",\"quantity\":5}\n",
        "]\n",
        "toAdd=input(\"Enter item to add: \")\n",
        "howMuch=int(input(\"Enter quantity to add: \"))\n",
        "first_dict=Inventory[0]\n",
        "second_dict=Inventory[1]\n",
        "third_dict=Inventory[2]\n",
        "fourth_dict=Inventory[3]\n",
        "match toAdd:\n",
        "  case \"Gold Galleons\":\n",
        "    first_dict[\"quantity\"]=first_dict[\"quantity\"]+howMuch\n",
        "    print(first_dict[\"quantity\"], \"are the total galleons\")\n",
        "  case \"Silver Sickles\":\n",
        "    second_dict[\"quantity\"]=second_dict[\"quantity\"]+howMuch\n",
        "    print(second_dict[\"quantity\"], \"are the total sickles\")\n",
        "  case \"Bronze Knuts\":\n",
        "    third_dict[\"quantity\"]=third_dict[\"quantity\"]+howMuch\n",
        "    print(third_dict[\"quantity\"], \"are the total knuts\")\n",
        "  case \"Potion Bottles\":\n",
        "    fourth_dict[\"quantity\"]=fourth_dict[\"quantity\"]+howMuch\n",
        "    print(fourth_dict[\"quantity\"], \"are the total bottles\")\n",
        "  case _ :\n",
        "    print(Inventory)\n",
        "\n",
        "worth=first_dict[\"quantity\"]+round((second_dict[\"quantity\"])/29,3)+round((third_dict[\"quantity\"])/29,3)\n",
        "print(\"Total worth of inventory is \"+str(worth)+\" galleons.\")\n",
        "print(Inventory)"
      ],
      "metadata": {
        "id": "e5kW3LaPKKsv",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "b4ce528f-9625-42b9-923d-0a83baee990e"
      },
      "execution_count": 9,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Enter item to add: Gold Galleons\n",
            "Enter quantity to add: 100\n",
            "200 are the total galleons\n",
            "Total worth of inventory is 286.207 galleons.\n",
            "[{'name': 'Gold Galleons', 'quantity': 200}, {'name': 'Silver Sickles', 'quantity': 500}, {'name': 'Bronze Knuts', 'quantity': 2000}, {'name': 'Potion Bottles', 'quantity': 5}]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Other Data Types"
      ],
      "metadata": {
        "id": "H_rnw_40cDsk"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Tuples are ordered, immutable collections of elements. They are defined using parentheses ()."
      ],
      "metadata": {
        "id": "EtCbJ8xCkGKH"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "my_tuple = (1, 2, \"apple\", True)\n",
        "print(my_tuple)\n",
        "# try changing the length of the tuple or value of any element in the tuple"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "t5kdNQHUkIbL",
        "outputId": "6cd40858-2a1a-425f-df16-a4ef255dacc5"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "(1, 2, 'apple', True)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Sets are unordered collections of unique elements. They are defined using curly braces {}. Sets are mutable."
      ],
      "metadata": {
        "id": "IbRqEFb0kji9"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "my_set = set()\n",
        "my_set.add(1)\n",
        "my_set.add(2)\n",
        "my_set.add(3)\n",
        "my_set.add(2) # won't add duplicate\n",
        "print(my_set)\n",
        "another_set = {3,4,5}\n",
        "print(my_set.intersection(another_set))\n",
        "print(my_set.union(another_set))\n",
        "print(my_set.difference(another_set))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "9hNnTNd5kZC9",
        "outputId": "25ba5a56-0ad7-43c9-8630-d82d797559e7"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "{1, 2, 3}\n",
            "{3}\n",
            "{1, 2, 3, 4, 5}\n",
            "{1, 2}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Frozensets are immutable versions of sets. They are defined using the frozenset() constructor."
      ],
      "metadata": {
        "id": "Hi4RWSdCk3rQ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "my_frozenset = frozenset([1, 2, 3, \"apple\"])\n",
        "print(my_frozenset)\n",
        "# try changing it in any manner"
      ],
      "metadata": {
        "id": "03RkH6xQk52s",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "eb17ed86-cb6b-440d-f5ca-0f4d83b6c880"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "frozenset({1, 2, 3, 'apple'})\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Functions"
      ],
      "metadata": {
        "id": "Cxwpc2u4cI9y"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "One great thing about python is no need to define any access specifiers or any other technical jargon while creating our own functions. Just use 'def' and be done with it!"
      ],
      "metadata": {
        "id": "srIvr421cij7"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "def hello(to=\"world\"): # default parameter implementation done here\n",
        "    print(\"hello,\", to)\n",
        "hello(\"hagrid\")\n",
        "hello()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "yyoi-F2CcMOY",
        "outputId": "a369e7ce-3fcd-435b-a234-726db5a2b6b4"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "hello, hagrid\n",
            "hello, world\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "# returning values is the same as before\n",
        "def main():\n",
        "    x = int(input(\"What's x? \"))\n",
        "    print(\"x squared is\", square(x))\n",
        "\n",
        "def square(n):\n",
        "    return n * n\n",
        "\n",
        "main()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "5P-SQ_Cyc9Hh",
        "outputId": "9cbd0074-ba69-49dd-ce29-be9cdeca5b7f"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What's x? 7\n",
            "x squared is 49\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "**Excerise time**\n",
        "\n",
        "Try to implement the following pattern:\n",
        "\n",
        "A\n",
        "\n",
        "BC\n",
        "\n",
        "DEF\n",
        "\n",
        "GHIJ\n",
        "\n",
        "KLMNO"
      ],
      "metadata": {
        "id": "TcO4hkjWdiF6"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# write your code here\n",
        "def print_pattern():\n",
        "    start_char = ord('A')\n",
        "    num_rows = 5\n",
        "\n",
        "    for row in range(1, num_rows + 1):\n",
        "\n",
        "        for _ in range(row):\n",
        "            print(chr(start_char), end=\"\")\n",
        "            start_char += 1\n",
        "\n",
        "        print()\n",
        "\n",
        "print_pattern()\n"
      ],
      "metadata": {
        "id": "vR4tO3uLdVWf",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "178a18f8-eb5e-4907-99f5-ac807f11e832"
      },
      "execution_count": 10,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "A\n",
            "BC\n",
            "DEF\n",
            "GHIJ\n",
            "KLMNO\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Important inbuilt functions"
      ],
      "metadata": {
        "id": "emAemZC3d9Zf"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Lambda is used to create small, anonymous functions. This is important concept in the functional programming paradigm in python. See this [link](https://realpython.com/python-functional-programming/) if feeling comfortable and curious!"
      ],
      "metadata": {
        "id": "z_-Kf65bfI-C"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "square = lambda x: x ** 2\n",
        "print(square(5))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "yifn-TUaetaI",
        "outputId": "bcf72c59-e957-46d1-ad88-b47177e63e6d"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "25\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Map applies a given function to each item of an iterable, returning a new iterable with the results."
      ],
      "metadata": {
        "id": "a5h9Y48jgsx7"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "numbers = [1, 2, 3, 4, 5]\n",
        "squared_numbers = list(map(lambda x: x ** 2, numbers))\n",
        "print(squared_numbers)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "mnZm9dpjfg3S",
        "outputId": "cf4c9317-5053-4c8d-a576-4bcd7c10a288"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1, 4, 9, 16, 25]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Filter creates a new iterable with items from the original that satisfy a given condition."
      ],
      "metadata": {
        "id": "qIxBKzkjiRO3"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "even_numbers = list(filter(lambda x: x % 2 == 0, numbers))\n",
        "print(even_numbers)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "owgE--UGiTjS",
        "outputId": "d0c1c398-b335-4ac9-8731-06af74ca8882"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[2, 4]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Reduce cumulatively applies a function to the items of an iterable, reducing it to a single value."
      ],
      "metadata": {
        "id": "dThe6F8qiI4g"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "from functools import reduce\n",
        "product = reduce(lambda x, y: x * y, numbers)\n",
        "print(product)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "uh2J1xr8iLsX",
        "outputId": "9f985513-f40f-4ee4-ec7e-65febaa56b05"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "120\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Python's math module provides a comprehensive set of mathematical functions, including:\n",
        "\n",
        "Basic arithmetic: abs(), ceil(), floor(), max(), min(), pow(), round(), sqrt()\n",
        "\n",
        "Trigonometric functions: sin(), cos(), tan(), asin(), acos(), atan(), degrees(), radians()\n",
        "\n",
        "Logarithmic and exponential functions: log(), log10(), exp()\n",
        "\n",
        "Number-theoretic functions: factorial(), gcd(), fmod()"
      ],
      "metadata": {
        "id": "9orkBAciidR5"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "x = -5\n",
        "absolute_value = abs(x)\n",
        "print(absolute_value)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "b8ARCEsJicwX",
        "outputId": "95c3cea7-3d28-45e3-e00e-6526ab5ae672"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "5\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "import math\n",
        "number = 3.14159\n",
        "rounded_down = math.floor(number)\n",
        "rounded_up = math.ceil(number)\n",
        "print(rounded_down, rounded_up)\n",
        "x = 24\n",
        "y = 36\n",
        "gcd_value = math.gcd(x, y)\n",
        "print(gcd_value)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "vPzizSSLjS5Z",
        "outputId": "61b5b0d5-213a-4237-c394-587e60a09a90"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "3 4\n",
            "12\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "**Exercise Time**\n",
        "\n",
        "- Define a dictionary for each Avenger containing attributes like name,\n",
        "superpower, strength, intelligence, and speed.\n",
        "- Store these dictionaries in a list.\n",
        "- Use filter or list comprehension to select Avengers based on specific criteria (e.g., strength greater than 4).\n",
        "- Create a new list to represent the assembled team.\n",
        "- Calculate the average strength, intelligence, and speed of the team using reduce.\n",
        "- Find the strongest, smartest, and fastest Avenger on the team.\n",
        "- Create a function that suggests a mission based on the team's overall attributes.\n",
        "- For example, a team with high intelligence might be suggested for a tactical mission."
      ],
      "metadata": {
        "id": "H9B5QQ4MP6sL"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# write your code here\n",
        "from functools import reduce\n",
        "\n",
        "avengers = [\n",
        "    {\"name\": \"Iron Man\", \"superpower\": \"Genius Intellect\", \"strength\": 7, \"intelligence\": 10, \"speed\": 6},\n",
        "    {\"name\": \"Thor\", \"superpower\": \"God of Thunder\", \"strength\": 10, \"intelligence\": 6, \"speed\": 8},\n",
        "    {\"name\": \"Hulk\", \"superpower\": \"Super Strength\", \"strength\": 10, \"intelligence\": 5, \"speed\": 5},\n",
        "    {\"name\": \"Black Widow\", \"superpower\": \"Espionage\", \"strength\": 5, \"intelligence\": 8, \"speed\": 7},\n",
        "    {\"name\": \"Captain America\", \"superpower\": \"Super Soldier\", \"strength\": 6, \"intelligence\": 7, \"speed\": 6},\n",
        "    {\"name\": \"Hawkeye\", \"superpower\": \"Expert Marksman\", \"strength\": 4, \"intelligence\": 6, \"speed\": 6}\n",
        "]\n",
        "strong_avengers = [avenger for avenger in avengers if avenger[\"strength\"] > 4]\n",
        "\n",
        "def calculate_averages(team):\n",
        "    total_strength = reduce(lambda acc, avenger: acc + avenger[\"strength\"], team, 0)\n",
        "    total_intelligence = reduce(lambda acc, avenger: acc + avenger[\"intelligence\"], team, 0)\n",
        "    total_speed = reduce(lambda acc, avenger: acc + avenger[\"speed\"], team, 0)\n",
        "    num_avengers = len(team)\n",
        "    avg_strength = total_strength / num_avengers\n",
        "    avg_intelligence = total_intelligence / num_avengers\n",
        "    avg_speed = total_speed / num_avengers\n",
        "    return avg_strength, avg_intelligence, avg_speed\n",
        "\n",
        "def find_extremes(team):\n",
        "    strongest = max(team, key=lambda avenger: avenger[\"strength\"])\n",
        "    smartest = max(team, key=lambda avenger: avenger[\"intelligence\"])\n",
        "    fastest = max(team, key=lambda avenger: avenger[\"speed\"])\n",
        "    return strongest, smartest, fastest\n",
        "\n",
        "def suggest_mission(avg_strength, avg_intelligence, avg_speed):\n",
        "    if avg_intelligence > avg_strength and avg_intelligence > avg_speed:\n",
        "        return \"Tactical Mission\"\n",
        "    elif avg_strength > avg_intelligence and avg_strength > avg_speed:\n",
        "        return \"Heavy Combat Mission\"\n",
        "    elif avg_speed > avg_strength and avg_speed > avg_intelligence:\n",
        "        return \"Reconnaissance Mission\"\n",
        "    else:\n",
        "        return \"General Mission\"\n",
        "\n",
        "avg_strength, avg_intelligence, avg_speed = calculate_averages(strong_avengers)\n",
        "\n",
        "strongest_avenger, smartest_avenger, fastest_avenger = find_extremes(strong_avengers)\n",
        "\n",
        "mission_suggestion = suggest_mission(avg_strength, avg_intelligence, avg_speed)\n",
        "\n",
        "print(f\"Strongest Avenger: {strongest_avenger['name']}\")\n",
        "print(f\"Smartest Avenger: {smartest_avenger['name']}\")\n",
        "print(f\"Fastest Avenger: {fastest_avenger['name']}\")\n",
        "print(f\"Average Strength: {avg_strength:.2f}\")\n",
        "print(f\"Average Intelligence: {avg_intelligence:.2f}\")\n",
        "print(f\"Average Speed: {avg_speed:.2f}\")\n",
        "print(f\"Suggested Mission: {mission_suggestion}\")\n"
      ],
      "metadata": {
        "id": "GzJYdlIIQQ2R",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "089daa5a-3d9b-4147-e740-769ef7950122"
      },
      "execution_count": 11,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Strongest Avenger: Thor\n",
            "Smartest Avenger: Iron Man\n",
            "Fastest Avenger: Thor\n",
            "Average Strength: 7.60\n",
            "Average Intelligence: 7.20\n",
            "Average Speed: 6.40\n",
            "Suggested Mission: Heavy Combat Mission\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Exceptions"
      ],
      "metadata": {
        "id": "Byu7Tzg0QSmI"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Exceptions are things that go wrong within our coding. You can learn more in Python’s documentation of [Errors and Exceptions](https://docs.python.org/3/tutorial/errors.html).\n",
        "\n",
        "\n",
        "In Python try and except are ways of testing out user input before something goes wrong. Try giving 'cat' as input."
      ],
      "metadata": {
        "id": "6sld1ZtrQ2Le"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "try:\n",
        "    x = int(input(\"What's x? \"))\n",
        "    print(f\"x is {x}\")\n",
        "except ValueError:\n",
        "    print(\"x is not an integer\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Oo7fhBMQQfv7",
        "outputId": "83c1f9f3-a2be-43f5-9ce3-06def6c4f67e"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What's x? cat\n",
            "x is not an integer\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "This is still not the best way to implement this code.\n",
        "Notice that we are trying to do two lines of code. For best practice, we should only try the fewest lines of code possible that we are concerned could fail. Adjust your code as follows:"
      ],
      "metadata": {
        "id": "-5rbcYu0RowT"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "try:\n",
        "    x = int(input(\"What's x? \"))\n",
        "except ValueError:\n",
        "    print(\"x is not an integer\")\n",
        "print(f\"x is {x}\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "FMa5N9u6RakE",
        "outputId": "ab7692dc-ba69-421e-96cc-ba69172d6283"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What's x? cat\n",
            "x is not an integer\n",
            "x is 24\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice that while this accomplishes our goal of trying as few lines as possible, we now face a new error! We face a NameError where x is not defined (to _undefine_ x, run `del x`). Look at this code and consider: Why is x not defined in some cases?\n",
        "\n",
        "It turns out that there is another way to implement try that could catch errors of this nature. Adjust your code as follows:"
      ],
      "metadata": {
        "id": "JmmfKqQmVKCG"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "try:\n",
        "    x = int(input(\"What's x?\"))\n",
        "except ValueError:\n",
        "    print(\"x is not an integer\")\n",
        "else:\n",
        "    print(f\"x is {x}\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "ooOnY8V2VSMf",
        "outputId": "76a3f31a-8911-42b9-ec5d-b3a026a2a852"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What's x?cat\n",
            "x is not an integer\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Regular Expression"
      ],
      "metadata": {
        "id": "V4loeV3FWKOx"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "It turns out that Python has an existing library called re that has a number of built-in functions that can validate user inputs against patterns.\n",
        "One of the most versatile functions within the library re is search.\n",
        "The search library follows the signature re.search(pattern, string, flags=0)."
      ],
      "metadata": {
        "id": "WKeZR_3JWRIm"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import re\n",
        "\n",
        "email = input(\"What's your email? \").strip()\n",
        "\n",
        "if re.search(\"@\", email):\n",
        "    print(\"Valid\")\n",
        "else:\n",
        "    print(\"Invalid\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "QaAVm-Z6WMck",
        "outputId": "ba89e1d8-5f16-4865-ef0e-6497d61cbcf2"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What's your email? username@mail.com\n",
            "Valid\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "We can further our program’s functionality. However, we need to advance our vocabulary around validation. It turns out that in the world of regular expressions there are certain symbols that allow us to identify patterns. At this point, we have only been checking for specific pieces of text like @. It so happens that many special symbols can be passed to the compiler for the purpose of engaging in validation. A non-exhaustive list of those patterns is as follows:\n",
        "\n",
        "\n",
        ".   any character except a new line\n",
        "\n",
        "\\*   0 or more repetitions\n",
        "\n",
        "\\+   1 or more repetitions\n",
        "\n",
        "?   0 or 1 repetition\n",
        "\n",
        "{m} m repetitions\n",
        "\n",
        "{m,n} m-n repetitions"
      ],
      "metadata": {
        "id": "u5cDIP3_WXIC"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import re\n",
        "\n",
        "email = input(\"What's your email? \").strip()\n",
        "\n",
        "if re.search(r\".+@.+\\.com\", email):\n",
        "    print(\"Valid\")\n",
        "else:\n",
        "    print(\"Invalid\")\n",
        "\n",
        "# Notice how we utilize the “escape character” or \\ as a way of regarding the . as part of our string instead of our validation expression.\n",
        "# Testing your code, you will notice that username@mail.com is regarded as valid, where username@mail?com is invalid."
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "OHHfSw9VWWeC",
        "outputId": "983444dd-2351-4bee-9679-0aa7cc9c6c9f"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What's your email? username@mail.com\n",
            "Valid\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "This is a good time to introduce “raw strings”. In Python, raw strings are strings that don’t format special characters—instead, each character is taken at face-value. Imagine \\n, for example. We’ve seen in an earlier lecture how, in a regular string, these two characters become one: a special newline character. In a raw string, however, \\n is treated not as \\n, the special character, but as a single \\ and a single n. Placing an r in front of a string tells the Python interpreter to treat the string as a raw string, similar to how placing an f in front of a string tells the Python interpreter to treat the string as a format string:"
      ],
      "metadata": {
        "id": "DVBrvD4RXBHD"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import re\n",
        "\n",
        "email = input(\"What's your email? \").strip()\n",
        "\n",
        "if re.search(r\"^.+@.+\\.com$\", email):\n",
        "    print(\"Valid\")\n",
        "else:\n",
        "    print(\"Invalid\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "w0-0zTqiX0TB",
        "outputId": "e938dc68-8f54-4f7d-884c-ad6e98ca44bb"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What's your email? username@mail.com\n",
            "Valid\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "You could type in a sentence such as My email address is malan@harvard.edu. and this whole sentence would be considered valid. We can be even more precise in our coding.\n",
        "It just so happens we have more special symbols at our disposal in validation:\n",
        "\n",
        "^   matches the start of the string\n",
        "\n",
        "$   matches the end of the string or just before the newline at the end of the string"
      ],
      "metadata": {
        "id": "9aMuULBFX_F3"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Recall that within the re.search function, there is a parameter for flags.\n",
        "Some built-in flag variables are:\n",
        "\n",
        "re.IGNORECASE\n",
        "\n",
        "re.MULTILINE\n",
        "\n",
        "re.DOTALL"
      ],
      "metadata": {
        "id": "wTzzyw7tYSn6"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import re\n",
        "\n",
        "email = input(\"What's your email? \").strip()\n",
        "\n",
        "if re.search(r\"^\\w+@\\w+\\.com$\", email, re.IGNORECASE):\n",
        "    print(\"Valid\")\n",
        "else:\n",
        "    print(\"Invalid\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "LxXqtAjtYTde",
        "outputId": "d1d11efe-2daa-4883-b187-d4c4d7464672"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "What's your email? username@mail.com\n",
            "Valid\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "For a quick guide to Regex, refer [this](https://support.google.com/a/answer/1371415)."
      ],
      "metadata": {
        "id": "yEEulZla-X71"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## OOPS"
      ],
      "metadata": {
        "id": "xgZNB4SSYhyN"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Classes are a way by which, in object-oriented programming, we can create our own type of data and give them names.\n",
        "\n",
        "A class is like a mold for a type of data – where we can invent our own data type and give them a name."
      ],
      "metadata": {
        "id": "1_THo49Cn7Mr"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "class Student:\n",
        "    ...\n",
        "\n",
        "\n",
        "def main():\n",
        "    student = get_student()\n",
        "    print(f\"{student.name} from {student.house}\")\n",
        "\n",
        "\n",
        "def get_student():\n",
        "    student = Student()\n",
        "    student.name = input(\"Name: \")\n",
        "    student.house = input(\"House: \")\n",
        "    return student\n",
        "\n",
        "\n",
        "if __name__ == \"__main__\": # this allows you to import this file to other files without causing it's code to run unintended\n",
        "    main()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Ff3IloRVn9BD",
        "outputId": "66cfbe11-2657-4716-db77-0f244d00cfb5"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Name: Harry Potter\n",
            "House: Gryffindor\n",
            "Harry Potter from Gryffindor\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice by convention that Student is capitalized. Further, notice the ... simply means that we will later return to finish that portion of our code. Further, notice that in get_student, we can create a student of class Student using the syntax student = Student(). Further, notice that we utilize “dot notation” to access attributes of this variable student of class Student.\n",
        "\n",
        "Any time you create a class and you utilize that blueprint to create something, you create what is called an “object” or an “instance”. In the case of our code, student is an object."
      ],
      "metadata": {
        "id": "UNpbWKbaoJSI"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "class Student:\n",
        "    def __init__(self, name, house):\n",
        "        self.name = name\n",
        "        self.house = house\n",
        "\n",
        "\n",
        "def main():\n",
        "    student = get_student()\n",
        "    print(f\"{student.name} from {student.house}\")\n",
        "\n",
        "\n",
        "def get_student():\n",
        "    name = input(\"Name: \")\n",
        "    house = input(\"House: \")\n",
        "    return Student(name, house)\n",
        "\n",
        "\n",
        "if __name__ == \"__main__\":\n",
        "    main()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Bm4O0rQ5pBr9",
        "outputId": "5ccbbab0-8c7f-49e3-912c-84b882c5cad9"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Name: Draco Malfoy\n",
            "House: Slytherin\n",
            "Draco Malfoy from Slytherin\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice that within Student, we standardize the attributes of this class. We can create a function within class Student, called a “method”, that determines the behavior of an object of class Student. Within this function, it takes the name and house passed to it and assigns these variables to this object. Further, notice how the constructor student = Student(name, house) calls this function within the Student class and creates a student. self refers to the current object that was just created.\n",
        "\n",
        "You can learn more in Python’s documentation of [classes](https://docs.python.org/3/tutorial/classes.html)."
      ],
      "metadata": {
        "id": "xZ-srXKspQud"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Object-oriented program encourages you to encapusulate all the functionality of a class within the class definition. What if something goes wrong? What if someone tries to type in something random? What if someone tries to create a student without a name?"
      ],
      "metadata": {
        "id": "22Son9xTplFZ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "class Student:\n",
        "    def __init__(self, name, house):\n",
        "        if not name:\n",
        "            raise ValueError(\"Missing name\")\n",
        "        if house not in [\"Gryffindor\", \"Hufflepuff\", \"Ravenclaw\", \"Slytherin\"]:\n",
        "            raise ValueError(\"Invalid house\")\n",
        "        self.name = name\n",
        "        self.house = house\n",
        "\n",
        "\n",
        "def main():\n",
        "    student = get_student()\n",
        "    print(f\"{student.name} from {student.house}\")\n",
        "\n",
        "\n",
        "def get_student():\n",
        "    name = input(\"Name: \")\n",
        "    house = input(\"House: \")\n",
        "    return Student(name, house)\n",
        "\n",
        "\n",
        "if __name__ == \"__main__\":\n",
        "    main()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "j-UdbU9rpn-S",
        "outputId": "fbcb1c1c-8958-47ca-8b50-308475896b1f"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Name: Hermione Granger\n",
            "House: Gryffindor\n",
            "Hermione Granger from Gryffindor\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice how we check now that a name is provided and a proper house is designated. It turns out we can create our own exceptions that alerts the programmer to a potential error created by the user called raise. In the case above, we raise ValueError with a specific error message.\n",
        "\n",
        "It just so happens that Python allows you to create a specific function by which you can print the attributes of an object. Notice how def __str__(self) provides a means by which a student is returned when called. Therefore, you can now, as the programmer, print an object, its attributes, or almost anything you desire related to that object.\n",
        "\n",
        "\\__str__ is a built-in method that comes with Python classes. It just so happens that we can create our own methods for a class as well!"
      ],
      "metadata": {
        "id": "UVS2gV_mpxcC"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "class Student:\n",
        "    def __init__(self, name, house, patronus=None):\n",
        "        if not name:\n",
        "            raise ValueError(\"Missing name\")\n",
        "        if house not in [\"Gryffindor\", \"Hufflepuff\", \"Ravenclaw\", \"Slytherin\"]:\n",
        "            raise ValueError(\"Invalid house\")\n",
        "        if patronus and patronus not in [\"Stag\", \"Otter\", \"Jack Russell terrier\"]:\n",
        "            raise ValueError(\"Invalid patronus\")\n",
        "        self.name = name\n",
        "        self.house = house\n",
        "        self.patronus = patronus\n",
        "\n",
        "    def __str__(self):\n",
        "        return f\"{self.name} from {self.house}\"\n",
        "\n",
        "    def charm(self):\n",
        "        match self.patronus:\n",
        "            case \"Stag\":\n",
        "                return \"🐴\"\n",
        "            case \"Otter\":\n",
        "                return \"🦦\"\n",
        "            case \"Jack Russell terrier\":\n",
        "                return \"🐶\"\n",
        "            case _:\n",
        "                return \"🪄\"\n",
        "\n",
        "\n",
        "def main():\n",
        "    student = get_student()\n",
        "    print(\"Expecto Patronum!\")\n",
        "    print(student.charm())\n",
        "\n",
        "\n",
        "def get_student():\n",
        "    name = input(\"Name: \")\n",
        "    house = input(\"House: \")\n",
        "    patronus = input(\"Patronus: \") or None\n",
        "    return Student(name, house, patronus)\n",
        "\n",
        "\n",
        "if __name__ == \"__main__\":\n",
        "    main()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "W9Rbq_VKp8Lc",
        "outputId": "9e82e2d7-63d7-4ac7-d6c8-2158ca9ed0c3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Name: Ron Weasley\n",
            "House: Gryffindor\n",
            "Patronus: Jack Russell terrier\n",
            "Expecto Patronum!\n",
            "🐶\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Decorators and Class Methods"
      ],
      "metadata": {
        "id": "7-k9bnedqHGU"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Properties can be utilized to harden our code. In Python, we define properties using function “decorators”, which begin with @"
      ],
      "metadata": {
        "id": "vVKiITvIqPVa"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "class Student:\n",
        "    def __init__(self, name, house):\n",
        "        self.name = name\n",
        "        self.house = house\n",
        "\n",
        "    def __str__(self):\n",
        "        return f\"{self.name} from {self.house}\"\n",
        "\n",
        "    # Getter for name\n",
        "    @property\n",
        "    def name(self):\n",
        "        return self._name\n",
        "\n",
        "    # Setter for name\n",
        "    @name.setter\n",
        "    def name(self, name):\n",
        "        if not name:\n",
        "            raise ValueError(\"Invalid name\")\n",
        "        self._name = name\n",
        "\n",
        "    @property\n",
        "    def house(self):\n",
        "        return self._house\n",
        "\n",
        "    @house.setter\n",
        "    def house(self, house):\n",
        "        if house not in [\"Gryffindor\", \"Hufflepuff\", \"Ravenclaw\", \"Slytherin\"]:\n",
        "            raise ValueError(\"Invalid house\")\n",
        "        self._house = house\n",
        "\n",
        "\n",
        "def main():\n",
        "    student = get_student()\n",
        "    print(student)\n",
        "\n",
        "\n",
        "def get_student():\n",
        "    name = input(\"Name: \")\n",
        "    house = input(\"House: \")\n",
        "    return Student(name, house)\n",
        "\n",
        "\n",
        "if __name__ == \"__main__\":\n",
        "    main()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "BC6ZsSHxqJqf",
        "outputId": "4fb7df4f-0607-4572-81fb-69607d5d347d"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Name: Cedric Diggory\n",
            "House: Hufflepuff\n",
            "Cedric Diggory from Hufflepuff\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice how we’ve written @property above a function called house. Doing so defines house as a property of our class. With house as a property, we gain the ability to define how some attribute of our class, _house, should be set and retrieved. Indeed, we can now define a function called a “setter”, via @house.setter, which will be called whenever the house property is set—for example, with student.house = \"Gryffindor\". Here, we’ve made our setter validate values of house for us. Notice how we raise a ValueError if the value of house is not any of the Harry Potter houses, otherwise, we’ll use house to update the value of _house. Why _house and not house? house is a property of our class, with functions via which a user attempts to set our class attribute. _house is that class attribute itself. The leading underscore, _, indicates to users they need not (and indeed, shouldn’t!) modify this value directly. _house should only be set through the house setter. Notice how the house property simply returns that value of _house, our class attribute that has presumably been validated using our house setter. When a user calls student.house, they’re getting the value of _house through our house “getter”."
      ],
      "metadata": {
        "id": "raNzzu4TqRiQ"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Sometimes, we want to add functionality to a class itself, not to instances of that class.\n",
        "@classmethod is a function that we can use to add functionality to a class as a whole.\n",
        "Here’s an example of _not_ using a class method."
      ],
      "metadata": {
        "id": "HYcwFUMnqi-w"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import random\n",
        "\n",
        "\n",
        "class Hat:\n",
        "    def __init__(self):\n",
        "        self.houses = [\"Gryffindor\", \"Hufflepuff\", \"Ravenclaw\", \"Slytherin\"]\n",
        "\n",
        "    def sort(self, name):\n",
        "        print(name, \"is in\", random.choice(self.houses))\n",
        "\n",
        "\n",
        "hat = Hat()\n",
        "hat.sort(\"Harry\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "sUY5Gn-jqqdU",
        "outputId": "5f6f294e-5880-4651-e9a3-f1473cf69325"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Harry is in Slytherin\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice how when we pass the name of the student to the sorting hat, it will tell us what house is assigned to the student. Notice that hat = Hat() instantiates a hat. The sort functionality is always handled by the instance of the class Hat. By executing hat.sort(\"Harry\"), we pass the name of the student to the sort method of the particular instance of Hat, which we’ve called hat.\n",
        "\n",
        "We may want, though, to run the sort function without creating a particular instance of the sorting hat (there’s only one, after all!). We can modify our code as follows:"
      ],
      "metadata": {
        "id": "z02F8u5fqyfs"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import random\n",
        "\n",
        "\n",
        "class Hat:\n",
        "\n",
        "    houses = [\"Gryffindor\", \"Hufflepuff\", \"Ravenclaw\", \"Slytherin\"]\n",
        "\n",
        "    @classmethod\n",
        "    def sort(cls, name):\n",
        "        print(name, \"is in\", random.choice(cls.houses))\n",
        "\n",
        "\n",
        "Hat.sort(\"Harry\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "4bQbH1IDqzId",
        "outputId": "6a4c98b6-9c1e-43f6-e553-d888e7f33c35"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Harry is in Ravenclaw\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice how the __init__ method is removed because we don’t need to instantiate a hat anywhere in our code. self, therefore, is no longer relevant and is removed. We specify this sort as a @classmethod, replacing self with cls. Finally, notice how Hat is capitalized by convention near the end of this code, because this is the name of our class."
      ],
      "metadata": {
        "id": "iWB9mSc4q1lk"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Returning back to our previous code we can modify our code as follows, addressing some missed opportunities related to @classmethods"
      ],
      "metadata": {
        "id": "vvoJNKAGq72q"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "class Student:\n",
        "    def __init__(self, name, house):\n",
        "        self.name = name\n",
        "        self.house = house\n",
        "\n",
        "    def __str__(self):\n",
        "        return f\"{self.name} from {self.house}\"\n",
        "\n",
        "    @classmethod\n",
        "    def get(cls):\n",
        "        name = input(\"Name: \")\n",
        "        house = input(\"House: \")\n",
        "        return cls(name, house)\n",
        "\n",
        "\n",
        "def main():\n",
        "    student = Student.get()\n",
        "    print(student)\n",
        "\n",
        "\n",
        "if __name__ == \"__main__\":\n",
        "    main()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "-v5eCpRaq-W1",
        "outputId": "09fc0ea8-765e-4bfd-95d5-3e70fdee2eae"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Name: Luna Lovegood\n",
            "House: Ravenclaw\n",
            "Luna Lovegood from Ravenclaw\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Inheritance"
      ],
      "metadata": {
        "id": "8x-2SzhkrCFL"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Inheritance is, perhaps, the most powerful feature of object-oriented programming.\n",
        "\n",
        "It just so happens that you can create a class that “inherits” methods, variables, and attributes from another class."
      ],
      "metadata": {
        "id": "ewHrxMOfrEgb"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "class Wizard:\n",
        "    def __init__(self, name):\n",
        "        if not name:\n",
        "            raise ValueError(\"Missing name\")\n",
        "        self.name = name\n",
        "\n",
        "    ...\n",
        "\n",
        "\n",
        "class Student(Wizard):\n",
        "    def __init__(self, name, house):\n",
        "        super().__init__(name)\n",
        "        self.house = house\n",
        "\n",
        "    ...\n",
        "\n",
        "\n",
        "class Professor(Wizard):\n",
        "    def __init__(self, name, subject):\n",
        "        super().__init__(name)\n",
        "        self.subject = subject\n",
        "\n",
        "    ...\n",
        "\n",
        "\n",
        "wizard = Wizard(\"Albus\")\n",
        "student = Student(\"Harry\", \"Gryffindor\")\n",
        "professor = Professor(\"Severus\", \"Defense Against the Dark Arts\")\n",
        "..."
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "ZjaLFOEGrDlK",
        "outputId": "1cf66970-eabc-47ca-c0ea-24e406ffe1c9"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "Ellipsis"
            ]
          },
          "metadata": {},
          "execution_count": 66
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice that there is a class above called Wizard and a class called Student. Further, notice that there is a class called Professor. Both students and professors have names. Also, both students and professors are wizards. Therefore, both Student and Professor inherit the characteristics of Wizard. Within the “child” class Student, Student can inherit from the “parent” or “super” class Wizard as the line super().__init__(name) runs the init method of Wizard. Finally, notice that the last lines of this code create a wizard called Albus, a student called Harry, and so on"
      ],
      "metadata": {
        "id": "_XJZ6WxsrLXw"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "While we have just introduced inheritance, we have been using this all along during our use of exceptions.\n",
        "It just so happens that exceptions come in a heirarchy, where there are children, parent, and grandparent classes. These are illustrated below:\n",
        "\n",
        "-- BaseException\n",
        "\n",
        "-- KeyboardInterrupt\n",
        "\n",
        "-- Exception\n",
        "\n",
        "-- ArithmeticError\n",
        "\n",
        "-- ZeroDivisionError\n",
        "\n",
        "-- AssertionError\n",
        "\n",
        "-- AttributeError\n",
        "\n",
        "-- EOFError\n",
        "\n",
        "-- ImportError\n",
        "\n",
        "-- ModuleNotFoundError\n",
        "\n",
        "-- LookupError\n",
        "\n",
        "-- KeyError\n",
        "\n",
        "-- NameError\n",
        "\n",
        "-- SyntaxError\n",
        "\n",
        "-- IndentationError\n",
        "\n",
        "-- ValueError\n",
        "\n",
        "You can learn more in Python’s documentation of [exceptions](https://docs.python.org/3/library/exceptions.html)."
      ],
      "metadata": {
        "id": "SK073-GHrQi-"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Operator Overloading"
      ],
      "metadata": {
        "id": "EKuCsISAsHvZ"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Some operators such as + and - can be “overloaded” such that they can have more abilities beyond simple arithmetic."
      ],
      "metadata": {
        "id": "Aqb074RMseqH"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "class Vault:\n",
        "    def __init__(self, galleons=0, sickles=0, knuts=0):\n",
        "        self.galleons = galleons\n",
        "        self.sickles = sickles\n",
        "        self.knuts = knuts\n",
        "\n",
        "    def __str__(self):\n",
        "        return f\"{self.galleons} Galleons, {self.sickles} Sickles, {self.knuts} Knuts\"\n",
        "\n",
        "    def __add__(self, other):\n",
        "        galleons = self.galleons + other.galleons\n",
        "        sickles = self.sickles + other.sickles\n",
        "        knuts = self.knuts + other.knuts\n",
        "        return Vault(galleons, sickles, knuts)\n",
        "\n",
        "\n",
        "potter = Vault(100, 50, 25)\n",
        "print(potter)\n",
        "\n",
        "weasley = Vault(25, 50, 100)\n",
        "print(weasley)\n",
        "\n",
        "total = potter + weasley\n",
        "print(total)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "aMo7jm0dshPb",
        "outputId": "b621e297-846d-4903-df08-78ea32937f6a"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "100 Galleons, 50 Sickles, 25 Knuts\n",
            "25 Galleons, 50 Sickles, 100 Knuts\n",
            "125 Galleons, 100 Sickles, 125 Knuts\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Notice how the __str__ method returns a formatted string. Further, notice how the __add__ method allows for the addition of the values of two vaults. self is what is on the left of the + operand. other is what is right of the +.\n",
        "\n",
        "You can learn more in Python’s documentation of [operator overloading](https://docs.python.org/3/reference/datamodel.html#special-method-names)."
      ],
      "metadata": {
        "id": "0xApFHuqsk4O"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## NumPy"
      ],
      "metadata": {
        "id": "_53ei20_veSA"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "### Introduction"
      ],
      "metadata": {
        "id": "tUlP1Kv3xyIe"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "NumPy is a popular library for storing arrays of numbers and performing computations on them. Not only this enables to write often more succint code, this also makes the code faster, since most NumPy routines are implemented in C for speed.\n",
        "\n",
        "To use NumPy in your program, you need to import it as follows"
      ],
      "metadata": {
        "id": "QegB5wZrwdNF"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import numpy as np"
      ],
      "metadata": {
        "id": "rTBQSBnIvjFx"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "NumPy arrays can be created from Python lists"
      ],
      "metadata": {
        "id": "2iV7B3OvwfhW"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "my_array = np.array([1, 2, 3])\n",
        "my_array"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "2D7waRnkwh0e",
        "outputId": "44a151e1-b596-4613-dd13-b56561fc2bcd"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([1, 2, 3])"
            ]
          },
          "metadata": {},
          "execution_count": 69
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "Sy2EvrxFriAG"
      },
      "source": [
        "NumPy supports array of arbitrary dimension. For example, we can create two-dimensional arrays (e.g. to store a matrix) as follows"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "wM-GYVMsrzNs",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "2fde9f6e-6c58-4c05-a65f-2d4e79b3e803"
      },
      "source": [
        "my_2d_array = np.array([[1, 2, 3], [4, 5, 6]])\n",
        "my_2d_array"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([[1, 2, 3],\n",
              "       [4, 5, 6]])"
            ]
          },
          "metadata": {},
          "execution_count": 70
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "-kZMzYsAsVAc"
      },
      "source": [
        "We can access individual elements of a 2d-array using two indices"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "4q8X86BbscPd",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "a057c85b-fa52-4550-9203-b1bf8c4b8930"
      },
      "source": [
        "my_2d_array[1, 2]"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "6"
            ]
          },
          "metadata": {},
          "execution_count": 71
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "OfVIKyxkTh0p"
      },
      "source": [
        "We can also access rows"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "CrKnDAtyTlYe",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "c0887b60-1ebe-47e3-ec4a-3f7c927b79d7"
      },
      "source": [
        "my_2d_array[1]"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([4, 5, 6])"
            ]
          },
          "metadata": {},
          "execution_count": 72
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "hskLBCp9ToCG"
      },
      "source": [
        "and columns"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "MOOFsLHhTozX",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "7960f381-53dc-4b40-cc93-a2d4c23829fb"
      },
      "source": [
        "my_2d_array[:, 2]"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([3, 6])"
            ]
          },
          "metadata": {},
          "execution_count": 73
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "keWK_5PHr9Q2"
      },
      "source": [
        "Arrays have a `shape` attribute"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "5QIo7l1Yr8m7",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "8c5dab54-fd14-4e6d-8863-04323c0e5510"
      },
      "source": [
        "print(my_array.shape)\n",
        "print(my_2d_array.shape)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "(3,)\n",
            "(2, 3)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "LmX0EDWVsoDY"
      },
      "source": [
        "Contrary to Python lists, NumPy arrays must have a type and all elements of the array must have the same type."
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "FZjOowkls57o",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "810a19ac-b5a1-43ca-a35d-ddb5ec2862d7"
      },
      "source": [
        "my_array.dtype"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "dtype('int64')"
            ]
          },
          "metadata": {},
          "execution_count": 75
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "i5AvLdf7tGnZ"
      },
      "source": [
        "The main types are `int32` (32-bit integers), `int64` (64-bit integers), `float32` (32-bit real values) and `float64` (64-bit real values)."
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "w8ym2qZCt9Nm"
      },
      "source": [
        "The `dtype` can be specified when creating the array"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "gXpM_FqruCVv",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "5482915f-9e8a-484d-f42d-116c970975ea"
      },
      "source": [
        "my_array = np.array([1, 2, 3], dtype=np.float64)\n",
        "my_array.dtype"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "dtype('float64')"
            ]
          },
          "metadata": {},
          "execution_count": 76
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "WueaRIONuTdS"
      },
      "source": [
        "We can create arrays of all zeros using"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "jbD8N1UauK8r",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "de02c96b-2268-4582-968b-9dbe4be6e202"
      },
      "source": [
        "zero_array = np.zeros((2, 3))\n",
        "zero_array"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([[0., 0., 0.],\n",
              "       [0., 0., 0.]])"
            ]
          },
          "metadata": {},
          "execution_count": 77
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "vn5go6qoudo4"
      },
      "source": [
        "and similarly for all ones using `ones` instead of `zeros`."
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "1kCRlhLJuvZ6"
      },
      "source": [
        "We can create a range of values using"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "EcQXDeEmuxpO",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "d68159a4-79e0-46f0-b935-f6901c9bfdaa"
      },
      "source": [
        "np.arange(5)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([0, 1, 2, 3, 4])"
            ]
          },
          "metadata": {},
          "execution_count": 78
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "ZvJECk6Iu3uF"
      },
      "source": [
        "or specifying the starting point"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "Pk3UzL3du_f8",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "d0fe4d80-59d3-4d7b-ffa8-8548037a2e26"
      },
      "source": [
        "np.arange(3, 5)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([3, 4])"
            ]
          },
          "metadata": {},
          "execution_count": 79
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "f1JtqFSivJKG"
      },
      "source": [
        "Another useful routine is `linspace` for creating linearly spaced values in an interval. For instance, to create 10 values in `[0, 1]`, we can use"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "udHHjGAHvOQM",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "5df30600-63aa-42f4-fe78-891aa9847d2d"
      },
      "source": [
        "np.linspace(0, 1, 10)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([0.        , 0.11111111, 0.22222222, 0.33333333, 0.44444444,\n",
              "       0.55555556, 0.66666667, 0.77777778, 0.88888889, 1.        ])"
            ]
          },
          "metadata": {},
          "execution_count": 80
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "WbcxAKobvgUT"
      },
      "source": [
        "Another important operation is `reshape`, for changing the shape of an array"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "4FPzTuDlvlLO",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "b162493a-219f-4161-e073-f7ef8af35dd1"
      },
      "source": [
        "my_array = np.array([1, 2, 3, 4, 5, 6])\n",
        "my_array.reshape(3, 2)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([[1, 2],\n",
              "       [3, 4],\n",
              "       [5, 6]])"
            ]
          },
          "metadata": {},
          "execution_count": 81
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "f9B0iCBlmfeY"
      },
      "source": [
        "### Basic operations"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "elQGgkqDxKLV"
      },
      "source": [
        "In NumPy, we express computations directly over arrays. This makes the code much more succint."
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "hkCU1T8ixghX"
      },
      "source": [
        "Arithmetic operations can be performed directly over arrays. For instance, assuming two arrays have a compatible shape, we can add them as follows"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "4AoiRq42x5mI",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "8be38623-8cef-43a1-918d-652d558c5e27"
      },
      "source": [
        "array_a = np.array([1, 2, 3])\n",
        "array_b = np.array([4, 5, 6])\n",
        "array_a + array_b"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([5, 7, 9])"
            ]
          },
          "metadata": {},
          "execution_count": 82
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "SyPqME2EyD4x"
      },
      "source": [
        "Compare this with the equivalent computation using a for loop"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "HxRFA_U2yfI-",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "57bb702e-93ef-40b5-835f-22476ddf2e55"
      },
      "source": [
        "array_out = np.zeros_like(array_a)\n",
        "for i in range(len(array_a)):\n",
        "  array_out[i] = array_a[i] + array_b[i]\n",
        "array_out"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([5, 7, 9])"
            ]
          },
          "metadata": {},
          "execution_count": 83
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "i2a-apX-zlPN"
      },
      "source": [
        "Not only this code is more verbose, it will also run much more slowly."
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "Qdn8MwpR0wX_"
      },
      "source": [
        "In NumPy, functions that operates on arrays in an element-wise fashion are called [universal functions](https://numpy.org/doc/stable/reference/ufuncs.html). For instance, this is the case of `np.sin`"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "JoanjiMu1BH5",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "920734e7-ae6c-4e4c-e41b-d6e84c7f4a9d"
      },
      "source": [
        "np.sin(array_a)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([0.84147098, 0.90929743, 0.14112001])"
            ]
          },
          "metadata": {},
          "execution_count": 84
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "jHljrPXg5h8W"
      },
      "source": [
        "Vector inner product can be performed using `np.dot`"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "TphR8oIx5ob9",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "3ac03b1f-48eb-47b8-feb0-ded1cf6ac740"
      },
      "source": [
        "np.dot(array_a, array_b)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "32"
            ]
          },
          "metadata": {},
          "execution_count": 85
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "lHInOiSW50OR"
      },
      "source": [
        "When the two arguments to `np.dot` are both 2d arrays, `np.dot` becomes matrix multiplication"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "QRbpbhPP6Up0",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "1cd6bade-4163-4590-abc6-79327e9e8607"
      },
      "source": [
        "array_A = np.random.rand(5, 3)\n",
        "array_B = np.random.randn(3, 4)\n",
        "np.dot(array_A, array_B)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([[ 0.92510627,  0.72724279,  0.2285308 , -1.6678703 ],\n",
              "       [ 0.26384989,  0.68615011, -0.19673115, -2.48532024],\n",
              "       [-0.25523571,  0.58114164, -0.48502101, -2.60626416],\n",
              "       [ 0.87058895,  0.54258527,  0.28212211, -1.36905661],\n",
              "       [ 1.65227773,  0.82872456,  0.66065529, -1.1827708 ]])"
            ]
          },
          "metadata": {},
          "execution_count": 86
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "odVawD9m6gwv"
      },
      "source": [
        "Matrix transpose can be done using `.transpose()` or `.T` for short"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "gvPe_JAO6mvF",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "de035b53-f828-4669-f059-a39ca95a0784"
      },
      "source": [
        "array_A.T"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([[0.86831463, 0.91675032, 0.7518938 , 0.80444126, 0.97714984],\n",
              "       [0.19205018, 0.38877229, 0.50249175, 0.06338447, 0.00670879],\n",
              "       [0.52019832, 0.24364295, 0.03943972, 0.41115379, 0.81296148]])"
            ]
          },
          "metadata": {},
          "execution_count": 87
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "JlWt3oFnE_E-"
      },
      "source": [
        "### Slicing and masking"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "e4aKKe7bFA65"
      },
      "source": [
        "Like Python lists, NumPy arrays support slicing"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "0kPhv2xcF1TP",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "7f21297b-d387-41f6-db78-cc432d284f6c"
      },
      "source": [
        "np.arange(10)[5:]"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([5, 6, 7, 8, 9])"
            ]
          },
          "metadata": {},
          "execution_count": 88
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "ITu2Wy4-GB2G"
      },
      "source": [
        "We can also select only certain elements from the array"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "8tlZzTB6GEyw",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "4c933421-6e36-4955-8428-75670df5144b"
      },
      "source": [
        "x = np.arange(10)\n",
        "mask = x >= 5\n",
        "x[mask]"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([5, 6, 7, 8, 9])"
            ]
          },
          "metadata": {},
          "execution_count": 89
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "NlGForCimjBL"
      },
      "source": [
        "### Exercises"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "Ur1UlSFPTu6O"
      },
      "source": [
        "**Exercise 1.** Create a 3d array of shape (2, 2, 2), containing 8 values. Access individual elements and slices."
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "v1ed4-vLUWXQ",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "e4fa4836-eb77-417b-d5af-9a739c193a77"
      },
      "source": [
        "import numpy as np\n",
        "\n",
        "array_3d = np.array([[[1, 2], [3, 4]], [[5, 6], [7, 8]]])\n",
        "print(\"3D Array:\")\n",
        "print(array_3d)\n",
        "element_1 = array_3d[0, 0, 0]\n",
        "element_2 = array_3d[1, 1, 1]\n",
        "print(\"\\nIndividual Elements:\")\n",
        "print(f\"Element at [0, 0, 0]: {element_1}\")\n",
        "print(f\"Element at [1, 1, 1]: {element_2}\")\n",
        "slice_1 = array_3d[0, :, :]\n",
        "slice_2 = array_3d[:, 1, :]\n",
        "print(\"\\nSlices:\")\n",
        "print(\"Slice at [0, :, :]:\")\n",
        "print(slice_1)\n",
        "print(\"\\nSlice at [:, 1, :]:\")\n",
        "print(slice_2)\n"
      ],
      "execution_count": 13,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "3D Array:\n",
            "[[[1 2]\n",
            "  [3 4]]\n",
            "\n",
            " [[5 6]\n",
            "  [7 8]]]\n",
            "\n",
            "Individual Elements:\n",
            "Element at [0, 0, 0]: 1\n",
            "Element at [1, 1, 1]: 8\n",
            "\n",
            "Slices:\n",
            "Slice at [0, :, :]:\n",
            "[[1 2]\n",
            " [3 4]]\n",
            "\n",
            "Slice at [:, 1, :]:\n",
            "[[3 4]\n",
            " [7 8]]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "s_ksfCDJzyxI"
      },
      "source": [
        "**Exercise 2.** Rewrite the [relu function](https://www.geeksforgeeks.org/activation-functions/) using [np.maximum](https://numpy.org/doc/stable/reference/generated/numpy.maximum.html). Check that it works on both a single value and on an array of values."
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "QtSTxH5Dz6f8"
      },
      "source": [
        "def relu_numpy(x):\n",
        "  return\n",
        "\n",
        "relu_numpy(np.array([1, -3, 2.5]))"
      ],
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "yd1ZoByo436x"
      },
      "source": [
        "**Exercise 3.** Compute the mean value of the features in the [iris dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_iris.html). Hint: use the `axis` argument on [np.mean](https://numpy.org/doc/stable/reference/generated/numpy.mean.html)."
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "fYFVobkP5JK6"
      },
      "source": [
        "from sklearn.datasets import load_iris\n",
        "X, y = load_iris(return_X_y=True)\n",
        "\n",
        "# Result should be an array of size 4."
      ],
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Matplotlib"
      ],
      "metadata": {
        "id": "4NUIwy9Fy520"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Matplotlib is a plotting library for Python.\n",
        "\n",
        "We start with a rudimentary plotting example."
      ],
      "metadata": {
        "id": "NnXeNKd-y9QJ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "from matplotlib import pyplot as plt\n",
        "\n",
        "x_values = np.linspace(-3, 3, 100)\n",
        "\n",
        "plt.figure()\n",
        "plt.plot(x_values, np.sin(x_values), label=\"Sinusoid\")\n",
        "plt.xlabel(\"x\")\n",
        "plt.ylabel(\"sin(x)\")\n",
        "plt.title(\"Matplotlib example\")\n",
        "plt.legend(loc=\"upper left\")\n",
        "plt.show()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 472
        },
        "id": "KydnXLCYy_J4",
        "outputId": "a6a75e25-61b8-4f47-cbb5-31a44018ad2e"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "display_data",
          "data": {
            "text/plain": [
              "<Figure size 640x480 with 1 Axes>"
            ],
            "image/png": "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\n"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "We continue with a rudimentary scatter plot example. This example displays samples from the iris dataset using the first two features. Colors indicate class membership (there are 3 classes)."
      ],
      "metadata": {
        "id": "rX5qjodQzEwt"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "from sklearn.datasets import load_iris\n",
        "X, y = load_iris(return_X_y=True)\n",
        "\n",
        "X_class0 = X[y == 0]\n",
        "X_class1 = X[y == 1]\n",
        "X_class2 = X[y == 2]\n",
        "\n",
        "plt.figure()\n",
        "plt.scatter(X_class0[:, 0], X_class0[:, 1], label=\"Class 0\", color=\"C0\")\n",
        "plt.scatter(X_class1[:, 0], X_class1[:, 1], label=\"Class 1\", color=\"C1\")\n",
        "plt.scatter(X_class2[:, 0], X_class2[:, 1], label=\"Class 2\", color=\"C2\")\n",
        "plt.show()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 433
        },
        "id": "1__969gozGYU",
        "outputId": "dc0e5f9a-fe00-4510-a4c8-79fcc64ae25a"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "display_data",
          "data": {
            "text/plain": [
              "<Figure size 640x480 with 1 Axes>"
            ],
            "image/png": "iVBORw0KGgoAAAANSUhEUgAAAiQAAAGgCAYAAACaOnwjAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAAA/JUlEQVR4nO3df3QU9b3/8dfuhiRGSC5YsokaAyo/GsBiVDT4i9YoFLT6vd/TUk8ESpXTevEKzT0t5F4tpbZN6I/0x7FfarlfAQWL9VSrWG+UoIgWFDDSG0yrUiHEShLuV5rwO2V3vn+sCWySTTKT3ZnZ2efjnBzPjp/h8/nsMNk3OzOfl88wDEMAAAAO8js9AAAAAAoSAADgOAoSAADgOAoSAADgOAoSAADgOAoSAADgOAoSAADgOAoSAADgOAoSAADgOAoSAADguEEVJFVVVfL5fFq8eHHMNmvWrJHP54v6yczMHEy3AADAY9Ks7rhz50498sgjuuyyy/ptm52drXfffbfrtc/nM9VXOBzWRx99pGHDhpneFwAAOMMwDB05ckTnn3++/P6+vwOxVJAcPXpUZWVlWrVqlb73ve/1297n8ykvL89KV5Kkjz76SAUFBZb3BwAAzmlqatKFF17YZxtLBcnChQs1a9YslZaWDqggOXr0qAoLCxUOh1VcXKwf/OAHmjBhQsz2p06d0qlTp7pedwYSNzU1KTs728qQAQCAzdrb21VQUKBhw4b129Z0QbJhwwbV1dVp586dA2o/btw4Pfroo7rsssvU1tamH//4x5o6dareeeedmNVSZWWlli9f3mN7dnY2BQkAAElmILdb+IzOrx8GoKmpSVdeeaU2bdrUde/ItGnTNHnyZP3sZz8b0J/xj3/8Q5/+9Kd155136qGHHuq1TfdvSDorrLa2NgoSAACSRHt7u3Jycgb0+W3qG5K33npLra2tKi4u7toWCoW0detWPfzwwzp16pQCgUCff8aQIUN0+eWXa+/evTHbZGRkKCMjw8zQAABAEjNVkNx0002qr6+P2jZ//nyNHz9eS5Ys6bcYkSIFTH19vWbOnGlupAAAwLNMFSTDhg3TxIkTo7ade+65Ou+887q2z507VxdccIEqKyslSd/97nd1zTXX6NJLL9Xf//53/ehHP1JjY6PuueeeOE0BAAAkO8vrkMRy4MCBqGeNDx8+rAULFqi5uVnDhw/XFVdcoW3btqmoqCjeXQMAgCRl6qZWp5i5KQYAALiDmc9vsmwAAIDjKEgAAIDj4n4PCYDECoUN7dj3sVqPnFTusExNGT1CAT8ZTwCSGwUJkERq9hzU8o0NOth2smtbfk6mlt1WpBkT8x0cGQAMDpdsgCRRs+eg7l1XF1WMSFJz20ndu65ONXsOOjQyABg8ChIgCYTChpZvbFBvj8R1blu+sUGhsOsfmgOAXlGQAElgx76Pe3wzcjZD0sG2k9qx72P7BgUAcURBAiSB1iOxixEr7QDAbShIgCSQOywzru0AwG0oSIAkMGX0COXnZCrWw70+RZ62mTJ6hJ3DAoC4oSABkkDA79Oy2yL5T92Lks7Xy24rYj0SAEmLggRIEjMm5mvlXcXKy4m+LJOXk6mVdxWzDgmApMbCaEASmTExXzcX5bFSKwDPoSABkkzA71PJJec5PQwAiCsu2QAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMdRkAAAAMelOT0AwEtCYUM79n2s1iMnlTssU1NGj1DA73N6WADgehQkQJzU7Dmo5RsbdLDtZNe2/JxMLbutSDMm5js4MgBwPy7ZAHFQs+eg7l1XF1WMSFJz20ndu65ONXsOOjQyAEgOFCTAIIXChpZvbJDRy//r3LZ8Y4NC4d5aAAAkChJg0Hbs+7jHNyNnMyQdbDupHfs+tm9QAJBkKEiAQWo9ErsYsdIOAFIRBQkwSLnDMuPaDgBSEQUJMEhTRo9Qfk6mYj3c61PkaZspo0fYOSwASCoUJMAgBfw+LbutSJJ6FCWdr5fdVsR6JADQBwoSIA5mTMzXyruKlZcTfVkmLydTK+8qZh0SAOgHC6MBcTJjYr5uLspjpVYAsICCBIijgN+nkkvOc3oYAJB0uGQDAAAcR0ECAAAcxyUbJC2SdQHAOyhIkJRI1gUAb+GSDZIOyboA4D0UJEgqJOsCgDdRkCCpkKwLAN5EQYKkQrIuAHgTBQmSCsm6AOBNFCRIKiTrAoA3UZAgqZCsCwDeREGCpEOyLgB4DwujISmRrAsA3kJBgqRFsi4AeAeXbAAAgOMoSAAAgOO4ZAOkAJKRAbjdoL4hqaqqks/n0+LFi/ts99RTT2n8+PHKzMzUpEmT9MILLwymWwAm1Ow5qOtWvKw7V72hRRt2685Vb+i6FS8TQgjAVSwXJDt37tQjjzyiyy67rM9227Zt05133qm7775bb7/9tu644w7dcccd2rNnj9WuAQwQycgAkoWlguTo0aMqKyvTqlWrNHz48D7b/vznP9eMGTP0zW9+U5/+9Kf10EMPqbi4WA8//LClAQMYGJKRASQTSwXJwoULNWvWLJWWlvbbdvv27T3aTZ8+Xdu3b4+5z6lTp9Te3h71A8AckpEBJBPTN7Vu2LBBdXV12rlz54DaNzc3KxgMRm0LBoNqbm6OuU9lZaWWL19udmgAzkIyMoBkYuobkqamJi1atEjr169XZmbi0lQrKirU1tbW9dPU1JSwvgCvIhkZQDIx9Q3JW2+9pdbWVhUXF3dtC4VC2rp1qx5++GGdOnVKgUAgap+8vDy1tLREbWtpaVFeXl7MfjIyMpSRkWFmaAC66UxGbm472et9JD5F8n9IRgbgBqa+IbnppptUX1+v3bt3d/1ceeWVKisr0+7du3sUI5JUUlKizZs3R23btGmTSkpKBjdyAH0iGRlAMjH1DcmwYcM0ceLEqG3nnnuuzjvvvK7tc+fO1QUXXKDKykpJ0qJFi3TjjTfqJz/5iWbNmqUNGzZo165d+vWvfx2nKQCIpTMZefnGhqgbXPNyMrXstiKSkQG4RtxXaj1w4ID8/jNfvEydOlVPPPGEHnjgAf37v/+7xowZo9///vc9ChsAiUEyMoBk4DMMw/WLELS3tysnJ0dtbW3Kzs52ejgAAGAAzHx+E64HAAAcR0ECAAAcR9ov0IeO02E9vn2/Gj8+rsIRWZpTMkrpadTxABBvFCRADJUvNGjVa/t0dtTL91/4sxZcP1oVM4ucGxgAeBAFCdCLyhca9MjWfT22hw11bacoAYD44btnoJuO02Gteq1nMXK2Va/tU8fpsE0jAgDvoyABunl8+/6oyzS9CRuRdgCA+KAgAbpp/Ph4XNsBAPpHQQJ0UzgiK67tAAD9oyABuplTMkr9raru90XaAQDig4IE6CY9za8F14/us82C60ezHgkAxBGP/QK96Hykt/s6JH6fWIcEABKAcD2gD6zUCgDWmfn85hsSoA/paX7dff3FTg8DADyPf+oBAADHUZAAAADHcckGrnCiI6QfvNCg/f/vuEadl6V/n1mkc9IDTg/LlUJhQzv2fazWIyeVOyxTU0aPUKC/55QBJJ1QOKS61jodOn5II7NGqji3WAF/fH8v2tHHQFGQwHELHtupTQ2tXa9fe196/I0DurkoV6vmXuXgyNynZs9BLd/YoINtJ7u25edkatltRZoxMd/BkQGIp9rGWlXtqFLL8ZaubcGsoJZOWarSwtKk6cMMLtnAUd2LkbNtamjVgsd22jwi96rZc1D3rquLKkYkqbntpO5dV6eaPQcdGhmAeKptrFX5lvKoQkGSWo+3qnxLuWoba5OiD7MoSOCYEx2hmMVIp00NrTrREbJpRO4VChtavrFBvT2j37lt+cYGhfpLBQTgaqFwSFU7qmT0crZ3bluxY4VCYeu/F+3owwoKEjjmBy80xLWdl+3Y93GPb0bOZkg62HZSO/Z9bN+gAMRdXWtdj28tzmbIUPPxZtW11rm6DysoSOCY/f9vYGm5A23nZa1HYhcjVtoBcKdDxw/FtZ1TfVhBQQLHjDpvYGm5A23nZbnDMuPaDoA7jcwaGdd2TvVhBQUJHPPvA8yDGWg7L5syeoTyczIV6+FenyJP20wZPcLOYQGIs+LcYgWzgvLFONt98ikvK0/FucWu7sMKChI45pz0gG4uyu2zzc1FuaxHIing92nZbZHCrPuvkM7Xy24rYj0SIMkF/AEtnbJUknoUDJ2vl0xZMqi1QuzowwoKEjhq1dyrYhYlrEMSbcbEfK28q1h5OdGXZfJyMrXyrmLWIQE8orSwVNXTqpWbFf27MZgVVPW06risEWJHH2aR9gtXYKXWgWOlViA1eGGlVjOf3xQkAAAgIcx8fnPJBgAAOI6CBAAAOI5wPbiCHfdFWOmD+zUAwB4UJHCcHQm2VvogWRcA7MMlGzjKjgRbK32QrAsA9qIggWPsSLC10gfJugBgPwoSOMaOBFsrfZCsCwD2oyCBY+xIsLXSB8m6AGA/ChI4xo4EWyt9kKwLAPajIIFj7EiwtdIHyboAYD8KEjjGjgRbK32QrAsA9qMggaPsSLC10gfJugBgL8L14Aqs1AoA3mPm85uVWuEKAb9PJZec57o+7BgXAIBLNgAAwAUoSAAAgOO4ZOMybrxngXsvADglFA6prrVOh44f0siskSrOLVbAH3B6WEgAChIXcWO6LCm5AJxS21irqh1Vajne0rUtmBXU0ilLVVpY6uDIkAg8ZeMSnemy3Q9G53cKTjxqamVMbpwHgORT21ir8i3lMrr9NvF98tukelo1RUkSMPP5zT0kLuDGdFlScgE4JRQOqWpHVY9iRFLXthU7VigUDtk9NCQQBYkLuDFdlpRcAE6pa62LukzTnSFDzcebVddaZ+OokGgUJC7gxnRZUnIBOOXQ8UNxbYfkQEHiAm5MlyUlF4BTRmaNjGs7JAcKEhdwY7osKbkAnFKcW6xgVrDrBtbufPIpLytPxbnFNo8MiURB4gJuTJclJReAUwL+gJZOWSpJPYqSztdLpixhPRKPoSBxCTemy5KSC8AppYWlqp5Wrdys3Kjtwawgj/x6FOuQuIwbVzhlpVYATmGl1uRm5vObggQAACQEC6MBAICkQkECAAAcR7geEqLjdFiPb9+vxo+Pq3BEluaUjFJ6Wuz612x7yZ33qbhxTACQDEzdQ7Jy5UqtXLlS+/fvlyRNmDBB3/72t/X5z3++1/Zr1qzR/Pnzo7ZlZGTo5ElzK3VyD0lyqXyhQate26ezI2v8PmnB9aNVMbNo0O0ldyYKu3FMAOCkhN1DcuGFF6qqqkpvvfWWdu3apc997nO6/fbb9c4778TcJzs7WwcPHuz6aWxsNNMlkkzlCw16ZGt0cSFJYUN6ZOs+Vb7QMKj20plE4e65Oc1tJ3XvujrV7DkYl7mY4cYxAUAyMVWQ3HbbbZo5c6bGjBmjsWPH6vvf/76GDh2qN954I+Y+Pp9PeXl5XT/BYHDQg4Y7dZwOa9Vr+/pss+q1feo4HbbUXnJnorAbxwQAycbyTa2hUEgbNmzQsWPHVFJSErPd0aNHVVhYqIKCgn6/Tel06tQptbe3R/3A/R7fvr/HNx3dhY1IOyvtJXcmCrtxTACQbEwXJPX19Ro6dKgyMjL09a9/Xc8884yKinq/zj9u3Dg9+uijevbZZ7Vu3TqFw2FNnTpVH374YZ99VFZWKicnp+unoKDA7DDhgMaPj5tqZ7a95M5EYTeOCQCSjemCZNy4cdq9e7fefPNN3XvvvZo3b54aGnpe55ekkpISzZ07V5MnT9aNN96op59+WiNHjtQjjzzSZx8VFRVqa2vr+mlqajI7TDigcESWqXZm20vuTBR245gAINmYLkjS09N16aWX6oorrlBlZaU+85nP6Oc///mA9h0yZIguv/xy7d27t892GRkZys7OjvqB+80pGaX+nnD1+yLtrLSX3Jko7MYxAUCyGfTCaOFwWKdOnRpQ21AopPr6euXn8wikF6Wn+bXg+tF9tllw/eiu9UXMtpfcmSjsxjEBQLIxVZBUVFRo69at2r9/v+rr61VRUaEtW7aorKxMkjR37lxVVFR0tf/ud7+rl156SR988IHq6up01113qbGxUffcc098ZwHXqJhZpK/dMLrHNx9+n/S1G3quK2K2veTORGE3jgkAkomplVpbW1s1d+5cHTx4UDk5Obrsssv04osv6uabb5YkHThwQH7/mRrn8OHDWrBggZqbmzV8+HBdccUV2rZtW8ybYOENFTOL9G+3jB/wyqtm20uRAuDmojxXrYrqxjEBQLIg7RcAACQEab8AACCpUJAAAADHkfbrMnakxVpJ1k10H1bm7ZX3yjPCIalxm3S0RRoalAqnSv5AXLsIhUOqa63ToeOHNDJrpIpzixXopw8r+wCwH/eQuIgdabFWknUT3YeVeXvlvfKMhuekmiVS+0dntmWfL81YIRV9IS5d1DbWqmpHlVqOt3RtC2YFtXTKUpUWlsZtHwDxY+bzm4LEJTrTYrsfjM5/78fj0dHOZN1YYj1mm8g+rMzbK++VZzQ8J/12rhTriHzpsUEXJbWNtSrfUi6jWx++T/qonlbdo8Cwsg+A+OKm1iRjR1qslWTdRPdhZd5eea88IxyKfDPS1xGpWRppZ1EoHFLVjqoehUWkh8i2FTtWKHRWH1b2AeAsChIXsCMt1kqybqL7sDJvr7xXntG4LfoyTQ+G1P63SDuL6lrroi659OzBUPPxZtW11g1qHwDOoiBxATvSYq0k6ya6Dyvz9sp75RlHY3/oW2rXi0PHD5luZ2UfAM6iIHEBO9JirSTrJroPK/P2ynvlGUOD8W3Xi5FZI023s7IPAGdRkLiAHWmxVpJ1E92HlXl75b3yjMKpkadp+joi2RdE2llUnFusYFaw62bUnj34lJeVp+Lc4kHtA8BZFCQuYEdarJVk3UT3YWXeXnmvPMMfiDzaKynmEZlRNaj1SAL+gJZOWfrJnxjdR+frJVOWRK0tYmUfAM7iN6pL2JEWayVZN9F9WJm3V94rzyj6QuTR3uxu73v2+XF55FeSSgtLVT2tWrlZuVHbg1nBmI/vWtkHgHNYh8RlvLL6KCu1piBWagXQDQujAQAAx7EwGgAASCoUJAAAwHGk/SIhzN7fYcf9IEhNodMdqqt/XIfaD2hk9kUqnjRHgbR0p4dlWsfpDj353pNqam9SQXaBZo+drfQknAcQC/eQIO7MJvHakdyL1FT7eqWq3luvlsCZ4jYYMrR0bJlKr6twcGTmVO+q1tqGtQobZ/KT/D6/5hXNU/mV5Q6ODOgb95DAMZ1JvN3zZprbTuredXWq2XNwUO2Bgap9vVLle9erpdtvuVa/VL53vWpfr3RmYCZV76rW6ndWRxUjkhQ2wlr9zmpV76p2aGRAfFGQIG7MJvHakdyL1BQ63aGq99ZH/h75oi/9GZ+8XvHeeoVOd9g/OBM6TndobcPaPtusbVirDpfPAxgIChLEjdkkXjuSe5Ga6uofj1ym8fV+H5Lh86k54FNd/eM2j8ycJ997ssc3I92FjbCefO9Jm0YEJA4FCeLGbBKvHcm9SE2H2g/EtZ1Tmtqb4toOcDMKEsSN2SReO5J7kZpGZl8U13ZOKcguiGs7wM0oSBA3ZpN47UjuRWoqnjRHwZAhX4yHCH2GobyQoeJJc2wemTmzx86W39f3r2m/z6/ZY2fbNCIgcShIEDdmk3jtSO5FagqkpWvp2DJJ6lGUdL5eMrbM9euRpKela17RvD7bzCuax3ok8AQKEsSV2SReO5J7kZpKr6tQ9aVlyu12T2gwLFVfmjzrkJRfWa75E+b3+KbE7/Nr/oT5rEMCz2BhNCQEK7XCLVipFXAOab8AAMBxrNQKAACSCgUJAABwHGm/Jthxn4PZPjpOh/X49v1q/Pi4CkdkaU7JKKWnOV9nck+IB4RDUuM26WiLNDQoFU6V/AGnR5VwVu45CYVDqmut06HjhzQya6SKc4sVcPi9sjIm0/vY8HfEje8tEoN7SAbIjkRas31UvtCgVa/t09lRL36ftOD60aqYWRSXMVlBeq8HNDwn1SyR2j86sy37fGnGCqnoC86NK8GspAPXNtaqakeVWo63nNknK6ilU5aqtLA04WOO15hM72PD3xE3vrcwh5ta46wzkbb7G9X5Kysej6ea7aPyhQY9snVfzD/vazc4U5TY8V4hwRqek347V4p1FL/0mCeLks504O6BfJ3rlvT2qHBtY63Kt5TL6PZe+T55r6qnVdv+wWllTKb3seHviBvfW5jHTa1xZEcirdk+Ok6Hteq12MWIJK16bZ86TvcdyhVvpPd6QDgU+VdvX0exZmmknYdYSQcOhUOq2lHV4wNTUte2FTtWKGTje2VlTKb3seHviBvfWyQeBUk/7EikNdvH49v3q7/P9LARaWcn0ns9oHFb9FfwPRhS+98i7TzESjpwXWtd1KWEHvvIUPPxZtW11sV9vLFYGZPpfWz4O+LG9xaJR0HSDzsSac320fjx8QG1H2i7eCG91wOOxv4QsNQuSVhJBz50/NDA9hlgu3iwMibT+9jwd8SN7y0Sj4KkH3Yk0prto3BE1oDaD7RdvJDe6wFDg/FtlySspAOPzBo5sH0G2C4erIzJ9D42/B1x43uLxKMg6YcdibRm+5hTMkr9PUHr90Xa2Yn0Xg8onBp5UqKvo5h9QaSdh1hJBy7OLVYwK9h1k2WPfeRTXlaeinOLEzLm3lgZk+l9bPg74sb3FolHQdIPOxJpzfaRnubXgutH9/lnLrh+tO3rkZDe6wH+QOSxTUkxj+KMKs+tR2IlHTjgD2jplKWRNt3eq87XS6YssXXNDCtjMr2PDX9H3PjeIvEoSAbAjkRas31UzCzS124Y3eObEr/PuUd+JdJ7PaHoC5HHNrO7Havs8z37yK9kLR24tLBU1dOqlZuVG71PVtCxx1KtjMn0Pjb8HXHje4vEYh0SE1ipdeBYqdUDWKmVlVpZqRWDxMJoAADAcSyMBgAAkgoFCQAAcBxpvy7DfSqAs9x6z0Ko44TqXntIh9oaNTKnUMXXP6hA+jlx7aOj44SefHOFmtoPqCD7Is2+eonS49wHEAv3kLgIicKAs9yaLlv77N2q+p9takk782/I4OnTWvqpqSq9/f/GpY/qmn/R2uatCp+1fL7fMDQv7waVz/g/cekDqYd7SJJQZ0pu9yyY5raTunddnWr2HLS9j85E4e65OWFDemTrPlW+0DDoMQFu0Zku2z1DpfV4q8q3lKu2sdaZcT17t8oPv6mWQPS3NK2BgMoPv6naZ+8edB/VNf+i1c1b1T2OMyxpdfNWVdf8y6D7APpDQeICJAoDznJrumyo44Sq/mdb3ynE/7NNoY4Tlvvo6Dihtc1bIy+6hwt+8npt81Z1DKIPYCAoSFyARGHAWW5Nl6177aHIZZq+UojT0lT32kOW+3jyzRWRyzQx+pDPp7DPpyffXNH7/wfihILEBUgUBpzl1nTZQ22NcW3Xm6YBJh0PtB1gFQWJC5AoDDjLremyI3MK49quNwUDTDoeaDvAKgoSFyBRGHCWW9Nli69/UMHTp/tOIT59WsXXP2i5j9lXL5HfMKRYD1wahvyGodlXL7HcBzAQFCQuQKIw4Cy3pssG0s/R0k9NjYwjVgrxp6YOaj2S9PRzNC/vhsiL7kXJJ6/n5d3AeiRIOD5NXIJEYcBZbk2XLb39/6p6+NXKDUU/4RMMhVQ9/Oq4rENSPuP/aH7eDT0+EPyS5rMOCWzCwmguw0qtgLNYqZWVWhE/pP0CAADHsVIrAABIKhQkAADAcSmb9mvlXg077u+wg9l7QlL5vVI4JDVuk462SEODUuFUKd73E5zukHaukg7vl4aPkq5aIKWlOzsmSaHTHaqrf1yH2g9oZPZFKp40R4E+xmXl3guzfbjViY4Tqq6rVmN7owqzC1VeXK5z+rr3wsIxtON42MHsuNw6D7MsnR8emftAmbqHZOXKlVq5cqX2798vSZowYYK+/e1v6/Of/3zMfZ566ik9+OCD2r9/v8aMGaMVK1Zo5syZpgYZ73tIrKTq2pHEawez6b2p/F6p4TmpZonU/tGZbdnnSzNWSEVfiE8fLz0obX9YMs7KBPL5pZL7pFt6WQ7cjjFJqn29UlXvrVdL4EwRGQwZWjq2TKXXVfRsbyEl12wfbnX/y/frlaZXemz/bMFn9YvP/aLnDhaOoR3Hww5mx+XWeZhl6fzwyNwTdlPrxo0bFQgENGbMGBmGobVr1+pHP/qR3n77bU2YMKFH+23btumGG25QZWWlbr31Vj3xxBNasWKF6urqNHHixIRMqD+dibfdJ915mvf2+KuVfdyoM703lu6P8qbye6WG56TfzpVizeRLjw2+AHjpQWlbLx9YnabeH12U2DEmRT78yveu7xHo1rnuRfWl0R+CnSm53YPpOtfv6O2RWbN9uFWsYqRTj6LEwjG043jYwey43DoPsyydHx6Zu2TzUzYjRozQj370I919d88I7NmzZ+vYsWN6/vnnu7Zdc801mjx5sn71q18NuI94FSShsKHrVrwcM2TOp8iaHK8v+VzX5QUr+7hRx+mwxj/4X30G5vl90l8e+rzS0/wp/V4pHJJ+NjH6X7BRfJF/0S6ut36p5HSH9P1g9DcjPboJSP/RHLl8Y8eYFLksMP2xYrX41WvYms8wFAxLNXPrFEhLVygc0vTfTY8ZTOeTT8GsoGr+d03XV81m+3CrEx0nNOU3U/ptt+POHZHLNxaOoR3Hww5mx+XWeZhl6fzwyNw72fKUTSgU0oYNG3Ts2DGVlJT02mb79u0qLY2u4qZPn67t27f3+WefOnVK7e3tUT/xYCVV144kXjuYTe9N5fdKjdv6+NCQJENq/1uknVU7V/VdjEiSEYq0s2tMkurqH49cFugrXTbgU13945H2FlJyzfbhVtV11ebaWTiGdhwPO5gdl1vnYZal88Mjc7fCdEFSX1+voUOHKiMjQ1//+tf1zDPPqKio9xU7m5ubFQwGo7YFg0E1Nzf32UdlZaVycnK6fgoKCswOs1dWUnXtSOK1g9n03lR+r3Q09i8DS+16c3i/uXZ2jEnSoQEmuna2s5KSa7YPt2psH1jCblc7C8fQjuNhB7Pjcus8zLJ0fnhk7laYLkjGjRun3bt3680339S9996refPmqaGhIa6DqqioUFtbW9dPU1NTXP5cK6m6diTx2sFsem8qv1caGuy/jZl2vRk+ylw7O8YkaeQAE10721lJyTXbh1sVZg8sYbernYVjaMfxsIPZcbl1HmZZOj88MncrTBck6enpuvTSS3XFFVeosrJSn/nMZ/Tzn/+817Z5eXlqaYn+V0FLS4vy8vL67CMjI0PZ2dlRP/FgJVXXjiReO5hN703l90qFUyPX8vuaSfYFkXZWXbUg8jRNX3yBSDu7xiSpeNIcBUNG3+myIUPFk+ZE2ltIyTXbh1uVF5eba2fhGNpxPOxgdlxunYdZls4Pj8zdikEvjBYOh3Xq1Kle/19JSYk2b94ctW3Tpk0x7zlJNCupunYk8drBbHpvKr9X8gcij2BKijmTGVWDW/sjLT3yaG9fShaeWY/EjjFJCqSla+nYssifGitddmxZ182mVlJyzfbhVuekn6PPFny2zzafLfjsmfVILBxDO46HHcyOy63zMMvS+eGRuVthqiCpqKjQ1q1btX//ftXX16uiokJbtmxRWVnkhJk7d64qKs48frZo0SLV1NToJz/5if7yl7/oO9/5jnbt2qX77uvnF3ECWUnVtSOJ1w5m03tT+b1S0Rcij2Bmdxtv9vlxe7xWtzwUebS3+zclvkDPR37tGpOk0usqVH1pmXK73XMbDPf+OK6VlFyzfbjVLz73i5hFSa/rkFg4hnYcDzuYHZdb52GWpfPDI3M3y9Rjv3fffbc2b96sgwcPKicnR5dddpmWLFmim2++WZI0bdo0jRo1SmvWrOna56mnntIDDzzQtTDaD3/4Q8cXRpNSe/VRVmo1gZVaWal1AFipdeBYqTW1Vmol7RcAADiOtF8AAJBUKEgAAIDjUjbt1wrP3BcBdzF7P4FN95CYZmVcNszd9HV4O95ftx5Dj/DCvRepiIJkgDyTYAt3MZv8alPar2lWxmXD3E0nptrx/rr1GHqEV1JyUxE3tQ6AZxJs4S5mk19tSvs1zcq4bJi76cRUO95ftx5Dj/BSSq5XcFNrHIXChpZvbOjx60M68ytl+cYGhfpLrgPOFg5F/pXc19+smqWRdlba28XKuGyYeygcUtWOqh4fTJE9IttW7FihkJ3vr1uPoUeYPuZwHQqSfngmwRbuYjb51aa0X9OsjMuGuZtOTLXj/XXrMfSIVE7J9QoKkn54JsEW7mI2+dWmtF/TrIzLhrmbTky14/116zH0iFROyfUKCpJ+eCbBFu5iNvnVprRf06yMy4a5m05MteP9desx9IhUTsn1CgqSfngmwRbuYjb51aa0X9OsjMuGuZtOTLXj/XXrMfSIVE7J9QoKkn54JsEW7mI2+dWmtF/TrIzLhrmbTky14/116zH0iFROyfUKCpIB8EyCLdzFbPKrTWm/plkZlw1zN52Yasf769Zj6BGpmpLrFaxDYgIrtSIhWKmVlVrdcgw9gpVa3YO0XwAA4DgWRgMAAEmFggQAADiOcD3AYaavd5/ukHaukg7vl4aPkq5aIKWlx7cPu5ici5V5mN2n43SHnnzvSTW1N6kgu0Czx85Wej/vryvvCXHjmFzKreeHW8eVKNxDAjjIdDLpSw9K2x+WjPCZbT6/VHKfdMtD8enDLibnYmUeZvep3lWttQ1rFT5rTH6fX/OK5qn8yvLe5+HG9F43jsml3Hp+uHVcZnFTK5AETCeTvvSgtO0Xsf/Aqff3+CB3bfqpyblYmYfZfap3VWv1O6tjDmn+hPk9ixI3pve6cUwu5dbzw63jsoKbWgGXM51Meroj8m1CX7b/MtLOah92MTkXK/Mwu0/H6Q6tbVjb55DWNqxVx1nvryvTe904Jpdy6/nh1nHZgYIEcIDpZNKdq6IvbfS6UyjSzmofdjE5FyvzMLvPk+89GXWZpjdhI6wn33vyzAY3pve6cUwu5dbzw63jsgMFCeAA08mkh/cP7A8+q51r009NzsXKPMzu09TeNKD2Ue3cmN7rxjG5lFvPD7eOyw4UJIADTCeTDh81sD/4rHauTT81ORcr8zC7T0F2wYDaR7VzY3qvG8fkUm49P9w6LjtQkAAOMJ1MetWCyBMoffEFIu2s9mEXk3OxMg+z+8weO1v+fsbk9/k1e+zsMxvcmN7rxjG5lFvPD7eOyw4UJIADTCeTpqVHHoftS8nCqDU8XJt+anIuVuZhdp/0tHTNK5rX55DmFc2LXo/Ejem9bhyTS7n1/HDruOxAQQI4xHQy6S0PRR6H7f4veV+g10d+LfVhF5NzsTIPs/uUX1mu+RPm9/imxO/z9/7Ir+TO9F43jsml3Hp+uHVcicY6JIDDWKmVlVoTwo1jcim3nh9uHZcZLIwGAAAcx8JoAAAgqVCQAAAAx5H2i+TllWvkNsyj4+RRPbm5XE1HP1TB0As1+6ZqpWcOjWsfbj0eZq/De+G6PZCMKEiQnLySZmrDPKqf+l9ae+x9hX2fPEJ4skk/3nCN5p07RuVffCYufbj1eJhNTPVKwiqQjLipFcnHK2mmNsyj+qn/pdXH3v/kjz1rTYNPTvv58ShKXHo8zCameilhFXALbmqFd3klzdSGeXScPKq1vRUjZ71ee+x9dZw8arkPtx4Ps4mpqZywCrgFBQmSi1fSTG2Yx5ObyyOXaboXI518PoV9Pj25uZcFvwbKpcfDbGJqKiesAm5BQYLk4pU0Uxvm0XT0w7i265VLj4fZxNRUTlgF3IKCBMnFK2mmNsyjYOiFcW3XK5ceD7OJqamcsAq4BQUJkotX0kxtmMfsm6rlN4yuG1h7MAz5DUOzb6q23Idbj4fZxNRUTlgF3IKCBMnFK2mmNswjPXOo5p07JvKie1Hyyet5544Z3HokLj0eZhNTUzlhFXALChIkH6+kmdowj/IvPqP5547pcaL7FadHfiXXHg+ziampmrAKuAXrkCB5uXRlUNNYqTWhWKkVcA5pvwAAwHEsjAYAAJIKBQkAAHAc4XpAPNlxH4WVPjxyfweQSlLt/KAgAeLFjsRbK314JIkXSCWpeH5wUysQD3Yk3lrpwyNJvEAq8dL5wU2tgJ3sSLy10odHkniBVJLK5wcFCTBYdiTeWunDI0m8QCpJ5fODggQYLDsSb6304ZEkXiCVpPL5QUECDJYdibdW+vBIEi+QSlL5/KAgAQbLjsRbK314JIkXSCWpfH5QkACDZUfirZU+PJLEC6SSVD4/KEiAeLAj8dZKHx5J4gVSSaqeH6xDAsQTK7WakmorUQJmeOH8IO0XAAA4joXRAABAUqEgAQAAjiNcD/2y5TqmS+9xMM2G+zu8cF3ZTqHTHaqrf1yH2g9oZPZFKp40R4G0dKeHZRrHHV5nqiCprKzU008/rb/85S8655xzNHXqVK1YsULjxo2Luc+aNWs0f/78qG0ZGRk6efKktRHDVrYkTro0jdY0G5J4UzEBdDBqX69U1Xvr1RI48/hk8O2faunYMpVeV+HgyMzhuCMVmLpk8+qrr2rhwoV64403tGnTJv3jH//QLbfcomPHjvW5X3Z2tg4ePNj109jYOKhBwx6diZPdcxVaj7eqfEu5ahtrB99JZxpt98yV9oOR7Q3PDb4PO1iZh8l9bDkeHlL7eqXK965XS7ffcq1+qXzvetW+XunMwEziuCNVDOopm0OHDik3N1evvvqqbrjhhl7brFmzRosXL9bf//53q93wlI0DQuGQpv9uesyQJ598CmYFVfO/a6x/bRwOST+b2EcAnC/ybcHiendfvrEyD5P72HI8PCR0ukPTHyuOFCO+nite+gxDwbBUM7fO1ZdvOO5IdrY9ZdPW1iZJGjFiRJ/tjh49qsLCQhUUFOj222/XO++802f7U6dOqb29PeoH9rIlcdKlabSm2ZDEm8oJoFbU1T8euUzTSzEiSYbPp+aAT3X1j9s8MnM47kgllguScDisxYsX69prr9XEiRNjths3bpweffRRPfvss1q3bp3C4bCmTp2qDz/8MOY+lZWVysnJ6fopKCiwOkxYZEvipEvTaE2zIYk3lRNArTjUfiCu7ZzCcUcqsVyQLFy4UHv27NGGDRv6bFdSUqK5c+dq8uTJuvHGG/X0009r5MiReuSRR2LuU1FRoba2tq6fpqYmq8OERbYkTro0jdY0G5J4UzkB1IqR2RfFtZ1TOO5IJZYKkvvuu0/PP/+8XnnlFV144YWm9h0yZIguv/xy7d27N2abjIwMZWdnR/3AXrYkTro0jdY0G5J4UzkB1IriSXMUDBnyxbhFzmcYygsZKp40x+aRmcNxRyoxVZAYhqH77rtPzzzzjF5++WWNHj3adIehUEj19fXKz8/vvzEcY0vipEvTaE2zIYk3lRNArQikpWvp2DJJ6lGUdL5eMrbM1Te0Shx3pBZTBcnChQu1bt06PfHEExo2bJiam5vV3NysEydOdLWZO3euKirOPN//3e9+Vy+99JI++OAD1dXV6a677lJjY6Puueee+M0CCWFL4qRL02hNsyGJN1UTQK0qva5C1ZeWKTccvT0YlqovTZ51SDjuSBWmHvv1xbhjffXq1frKV74iSZo2bZpGjRqlNWvWSJK+8Y1v6Omnn1Zzc7OGDx+uK664Qt/73vd0+eWXD3iQPPbrLFZqNYGVWl2HlVoB55D2CwAAHEfaLwAASCoUJAAAwHGk/aJ/Xrm/ww6nO6Sdq6TD+6Xho6SrFkhJeL8CANiNggR980oSrx1eelDa/rBknPVYx0sPSCX3Sbc85Ny4ACAJcMkGsXklidcOLz0obftFdDEiRV5v+0Xk/wMAYqIgQe/Cocg3I+rtIaxPttUsjbRLdac7It+M9GX7LyPtAAC9oiBB77ySxGuHnat6fjPSnRGKtAMA9IqCBL3zShKvHQ7vj287AEhBFCTonVeSeO0wfFR82wFACqIgQe+8ksRrh6sWSL5+TiVfINIOANArChL0zitJvHZIS4882tuXkoWsRwIAfaAgQWxeSeK1wy0PSVPv7/lNiS8Q2c46JADQJ8L10D9Wah04VmoFgC5mPr9ZqRX98wek0dc7PYrkkJYeuTwDADCFSzYAAMBxFCQAAMBxXLJJoFDY0I59H6v1yEnlDsvUlNEjFPDHeozWY1L1vpNUnbebcUyApEBBkiA1ew5q+cYGHWw72bUtPydTy24r0oyJ+X3s6QGpmhCcqvN2M44JkDS4ZJMANXsO6t51dVHFiCQ1t53UvevqVLPnoEMjs0GqJgSn6rzdjGMCJBUKkjgLhQ0t39jQV0aulm9sUCjs+qetzUvVhOBUnbebcUyApENBEmc79n3c45uRsxmSDrad1I59H9s3KLukakJwqs7bzTgmQNKhIImz1iOxixEr7ZJKqiYEp+q83YxjAiQdCpI4yx2WGdd2SSVVE4JTdd5uxjEBkg4FSZxNGT1C+TmZfWXkKj8n8giw56RqQnCqztvNOCZA0qEgibOA36dltxVJipmRq2W3FXlzPZJUTQhO1Xm7GccESDoUJAkwY2K+Vt5VrLyc6MsyeTmZWnlXsbfXIUnVhOBUnbebcUyApELabwKxUmsKro6ZqvN2M44J4Bgzn98UJAAAICHMfH5zyQYAADiOggQAADiOcD0AcRE63aG6+sd1qP2ARmZfpOJJcxRIS49vJ9wPAngWBQmAQat9vVJV761XS+DMTdvBt3+qpWPLVHpdRXw6IbkX8DQu2QAYlNrXK1W+d71auv02afVL5XvXq/b1ysF3QnIv4HkUJAAsC53uUNV76yP5ub7oR9qNT16veG+9Qqc7rHdCci+QEihIAFhWV/945DKNr/f1dQyfT80Bn+rqH7feCcm9QEqgIAFg2aH2A3Ft1yuSe4GUQEECwLKR2RfFtV2vSO4FUgIFCQDLiifNUTBkyBdjwWefYSgvZKh40hzrnZDcC6QEChIAlgXS0rV0bJkk9ShKOl8vGVs2uPVISO4FUgIFCYBBKb2uQtWXlik3HL09GJaqL43TOiQk9wKeR7gegLhgpVYA3Zn5/GalVgBxEUhL11WX353YTvwBafT1ie0DgCO4ZAMAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAAByX5vQA4FHhkNS4TTraIg0NSoVTJX/A6VEBAFzK1DcklZWVuuqqqzRs2DDl5ubqjjvu0Lvvvtvvfk899ZTGjx+vzMxMTZo0SS+88ILlASMJNDwn/WyitPZW6Xd3R/77s4mR7QAA9MJUQfLqq69q4cKFeuONN7Rp0yb94x//0C233KJjx47F3Gfbtm268847dffdd+vtt9/WHXfcoTvuuEN79uwZ9ODhQg3PSb+dK7V/FL29/WBkO0UJAKAXPsMwDKs7Hzp0SLm5uXr11Vd1ww039Npm9uzZOnbsmJ5//vmubddcc40mT56sX/3qVwPqp729XTk5OWpra1N2drbV4SLRwqHINyHdi5EuPin7fGlxPZdvACAFmPn8HtRNrW1tbZKkESNGxGyzfft2lZaWRm2bPn26tm/fHnOfU6dOqb29PeoHSaBxWx/FiCQZUvvfIu0AADiL5YIkHA5r8eLFuvbaazVx4sSY7ZqbmxUMBqO2BYNBNTc3x9ynsrJSOTk5XT8FBQVWhwk7HW2JbzsAQMqwXJAsXLhQe/bs0YYNG+I5HklSRUWF2traun6ampri3gcSYGiw/zZm2gEAUoalx37vu+8+Pf/889q6dasuvPDCPtvm5eWppSX6X8QtLS3Ky8uLuU9GRoYyMjKsDA1OKpwauUek/aCk3m5N+uQeksKpdo8MAOBypr4hMQxD9913n5555hm9/PLLGj16dL/7lJSUaPPmzVHbNm3apJKSEnMjhfv5A9KMFZ+88HX7n5+8nlHFDa0AgB5MFSQLFy7UunXr9MQTT2jYsGFqbm5Wc3OzTpw40dVm7ty5qqio6Hq9aNEi1dTU6Cc/+Yn+8pe/6Dvf+Y527dql++67L36zgHsUfUH60mNSdn709uzzI9uLvuDMuAAArmbqsV+fr/u/eiNWr16tr3zlK5KkadOmadSoUVqzZk3X/3/qqaf0wAMPaP/+/RozZox++MMfaubMmQMeJI/9JiFWagWAlGfm83tQ65DYhYIEAIDkY9s6JAAAAPFAQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxHQQIAABxnKe3Xbp2Lyba3tzs8EgAAMFCdn9sDWRQ+KQqSI0eOSJIKCgocHgkAADDryJEjysnJ6bNNUmTZhMNhffTRRxo2bFjMgD+3am9vV0FBgZqamlIuhydV556q85aYeyrOPVXnLTH3gczdMAwdOXJE559/vvz+vu8SSYpvSPx+vy688EKnhzEo2dnZKfcXtlOqzj1V5y0x91Sce6rOW2Lu/c29v29GOnFTKwAAcBwFCQAAcBwFSYJlZGRo2bJlysjIcHootkvVuafqvCXmnopzT9V5S8w93nNPiptaAQCAt/ENCQAAcBwFCQAAcBwFCQAAcBwFCQAAcBwFSRxVVVXJ5/Np8eLFMdusWbNGPp8v6iczM9O+QcbJd77znR7zGD9+fJ/7PPXUUxo/frwyMzM1adIkvfDCCzaNNr7Mzt0rx1yS/va3v+muu+7Seeedp3POOUeTJk3Srl27+txny5YtKi4uVkZGhi699FKtWbPGnsHGmdm5b9mypcdx9/l8am5utnHUgzdq1Khe57Fw4cKY+3jhXDc7by+d56FQSA8++KBGjx6tc845R5dccokeeuihfvNoBnuuJ8VKrclg586deuSRR3TZZZf12zY7O1vvvvtu1+tkWw6/04QJE1RbW9v1Oi0t9l+nbdu26c4771RlZaVuvfVWPfHEE7rjjjtUV1eniRMn2jHcuDIzd8kbx/zw4cO69tpr9dnPflb/9V//pZEjR+r999/X8OHDY+6zb98+zZo1S1//+te1fv16bd68Wffcc4/y8/M1ffp0G0c/OFbm3undd9+NWskyNzc3kUONu507dyoUCnW93rNnj26++WZ98Ytf7LW9V851s/OWvHGeS9KKFSu0cuVKrV27VhMmTNCuXbs0f/585eTk6P777+91n7ic6wYG7ciRI8aYMWOMTZs2GTfeeKOxaNGimG1Xr15t5OTk2Da2RFm2bJnxmc98ZsDtv/SlLxmzZs2K2nb11VcbX/va1+I8ssQzO3evHPMlS5YY1113nal9vvWtbxkTJkyI2jZ79mxj+vTp8RxawlmZ+yuvvGJIMg4fPpyYQTlk0aJFxiWXXGKEw+Fe/7+XzvWz9Tdvr5znhmEYs2bNMr761a9Gbfvnf/5no6ysLOY+8TjXuWQTBwsXLtSsWbNUWlo6oPZHjx5VYWGhCgoKdPvtt+udd95J8AgT4/3339f555+viy++WGVlZTpw4EDMttu3b+/x/kyfPl3bt29P9DATwszcJW8c8+eee05XXnmlvvjFLyo3N1eXX365Vq1a1ec+XjnuVubeafLkycrPz9fNN9+sP/7xjwkeaWJ1dHRo3bp1+upXvxrzX/9eOeZnG8i8JW+c55I0depUbd68We+9954k6U9/+pNef/11ff7zn4+5TzyOOwXJIG3YsEF1dXWqrKwcUPtx48bp0Ucf1bPPPqt169YpHA5r6tSp+vDDDxM80vi6+uqrtWbNGtXU1GjlypXat2+frr/+eh05cqTX9s3NzQoGg1HbgsFg0l1Pl8zP3SvH/IMPPtDKlSs1ZswYvfjii7r33nt1//33a+3atTH3iXXc29vbdeLEiUQPOW6szD0/P1+/+tWv9Lvf/U6/+93vVFBQoGnTpqmurs7GkcfX73//e/3973/XV77ylZhtvHSudxrIvL1ynkvS0qVL9eUvf1njx4/XkCFDdPnll2vx4sUqKyuLuU9cznVzX+TgbAcOHDByc3ONP/3pT13b+rtk011HR4dxySWXGA888EACRmifw4cPG9nZ2cZ//ud/9vr/hwwZYjzxxBNR2375y18aubm5dgwvofqbe3fJesyHDBlilJSURG3713/9V+Oaa66Juc+YMWOMH/zgB1Hb/vCHPxiSjOPHjydknIlgZe69ueGGG4y77rornkOz1S233GLceuutfbbx4rk+kHl3l6znuWEYxm9+8xvjwgsvNH7zm98Y//3f/2089thjxogRI4w1a9bE3Cce5zrfkAzCW2+9pdbWVhUXFystLU1paWl69dVX9Ytf/EJpaWlRN0TF0ll97t2714YRJ84//dM/aezYsTHnkZeXp5aWlqhtLS0tysvLs2N4CdXf3LtL1mOen5+voqKiqG2f/vSn+7xcFeu4Z2dn65xzzknIOBPBytx7M2XKlKQ77p0aGxtVW1ure+65p892XjvXBzrv7pL1PJekb37zm13fkkyaNElz5szRN77xjT6vBMTjXKcgGYSbbrpJ9fX12r17d9fPlVdeqbKyMu3evVuBQKDfPyMUCqm+vl75+fk2jDhxjh49qr/+9a8x51FSUqLNmzdHbdu0aZNKSkrsGF5C9Tf37pL1mF977bVRTxBI0nvvvafCwsKY+3jluFuZe292796ddMe90+rVq5Wbm6tZs2b12c4rx7zTQOfdXbKe55J0/Phx+f3R5UEgEFA4HI65T1yO+6C+10EP3S/ZzJkzx1i6dGnX6+XLlxsvvvii8de//tV46623jC9/+ctGZmam8c477zgwWuv+7d/+zdiyZYuxb98+449//KNRWlpqfOpTnzJaW1sNw+g57z/+8Y9GWlqa8eMf/9j485//bCxbtswYMmSIUV9f79QULDM7d68c8x07dhhpaWnG97//feP999831q9fb2RlZRnr1q3rarN06VJjzpw5Xa8/+OADIysry/jmN79p/PnPfzZ++ctfGoFAwKipqXFiCpZZmftPf/pT4/e//73x/vvvG/X19caiRYsMv99v1NbWOjGFQQmFQsZFF11kLFmypMf/8/K5bmbeXjnPDcMw5s2bZ1xwwQXG888/b+zbt894+umnjU996lPGt771ra42iTjXKUjirHtBcuONNxrz5s3rer148WLjoosuMtLT041gMGjMnDnTqKurs3+ggzR79mwjPz/fSE9PNy644AJj9uzZxt69e7v+f/d5G4Zh/Pa3vzXGjh1rpKenGxMmTDD+8Ic/2Dzq+DA7d68cc8MwjI0bNxoTJ040MjIyjPHjxxu//vWvo/7/vHnzjBtvvDFq2yuvvGJMnjzZSE9PNy6++GJj9erV9g04jszOfcWKFcYll1xiZGZmGiNGjDCmTZtmvPzyyzaPOj5efPFFQ5Lx7rvv9vh/Xj7XzczbS+d5e3u7sWjRIuOiiy4yMjMzjYsvvtj4j//4D+PUqVNdbRJxrvsMo5+l1wAAABKMe0gAAIDjKEgAAIDjKEgAAIDjKEgAAIDjKEgAAIDjKEgAAIDjKEgAAIDjKEgAAIDjKEgAAIDjKEgAAIDjKEgAAIDjKEgAAIDj/j+LQB9r38QNTAAAAABJRU5ErkJggg==\n"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "We see that samples belonging to class 0 can be linearly separated from the rest using only the first two features."
      ],
      "metadata": {
        "id": "zK5Qj5XqzKM7"
      }
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "1X6-g6zgCwJd"
      },
      "source": [
        "**Exercise 1.** Plot the relu and the [softplus](https://en.wikipedia.org/wiki/Rectifier_(neural_networks)#Softplus) functions on the same graph."
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "Ob6HZUX0DJ8y"
      },
      "source": [
        "# write your code here"
      ],
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "vpRGfz0aDW3l"
      },
      "source": [
        "What is the main difference between the two functions?"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "JjDeIufRAYVL"
      },
      "source": [
        "**Exercise 2.** Repeat the same scatter plot but using the [digits dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_digits.html) instead."
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "-JU3TXCBBB0c"
      },
      "source": [
        "from sklearn.datasets import load_digits\n",
        "X, y = load_digits(return_X_y=True)"
      ],
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "w7wPWdmXBQA2"
      },
      "source": [
        "Are pixel values good features for classifying samples?"
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Pandas"
      ],
      "metadata": {
        "id": "bJOKEBDJ0hb-"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Pandas is a powerful Python library used for data manipulation and analysis. It provides data structures like Series and DataFrame, which are essential for handling and analyzing structured data. Pandas makes data analysis tasks like cleaning, transforming, and aggregating data easier and more efficient.\n"
      ],
      "metadata": {
        "id": "svylv_MY0kY9"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import pandas as pd\n",
        "\n",
        "print(f\"Pandas Version: {pd.__version__}\") # checking the version of Pandas we are using"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "C_D9M6qp0oTn",
        "outputId": "1aafde80-cc1e-4794-9e8f-e350c4b9bfee"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Pandas Version: 2.1.4\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "A Series is a one-dimensional labeled array capable of holding any data type. In this example, we create a simple Series from a list of integers. The Series has both a data column and an index column."
      ],
      "metadata": {
        "id": "_gZS8GA50zpx"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "data = [10, 20, 30, 40, 50]\n",
        "series = pd.Series(data)\n",
        "series"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 241
        },
        "id": "mEKBBAT-03HW",
        "outputId": "57b00a7c-6c98-4567-bd50-9c027332f4c3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "0    10\n",
              "1    20\n",
              "2    30\n",
              "3    40\n",
              "4    50\n",
              "dtype: int64"
            ],
            "text/html": [
              "<div>\n",
              "<style scoped>\n",
              "    .dataframe tbody tr th:only-of-type {\n",
              "        vertical-align: middle;\n",
              "    }\n",
              "\n",
              "    .dataframe tbody tr th {\n",
              "        vertical-align: top;\n",
              "    }\n",
              "\n",
              "    .dataframe thead th {\n",
              "        text-align: right;\n",
              "    }\n",
              "</style>\n",
              "<table border=\"1\" class=\"dataframe\">\n",
              "  <thead>\n",
              "    <tr style=\"text-align: right;\">\n",
              "      <th></th>\n",
              "      <th>0</th>\n",
              "    </tr>\n",
              "  </thead>\n",
              "  <tbody>\n",
              "    <tr>\n",
              "      <th>0</th>\n",
              "      <td>10</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>1</th>\n",
              "      <td>20</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>2</th>\n",
              "      <td>30</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>3</th>\n",
              "      <td>40</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>4</th>\n",
              "      <td>50</td>\n",
              "    </tr>\n",
              "  </tbody>\n",
              "</table>\n",
              "</div><br><label><b>dtype:</b> int64</label>"
            ]
          },
          "metadata": {},
          "execution_count": 97
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "A DataFrame is a two-dimensional, size-mutable, and potentially heterogeneous tabular data structure with labeled axes (rows and columns). Here, we create a DataFrame from a dictionary where keys are column names, and values are lists of data."
      ],
      "metadata": {
        "id": "2wEMr4ZI09Rh"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "data = {\n",
        "    'Name': ['Alice', 'Bob', 'Charlie', 'David'],\n",
        "    'Age': [24, 27, 22, 32],\n",
        "    'City': ['New York', 'Los Angeles', 'Chicago', 'Houston']\n",
        "}\n",
        "\n",
        "df = pd.DataFrame(data)\n",
        "df"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 175
        },
        "id": "z4TVokpX0-fP",
        "outputId": "ad8223f8-9eed-46b3-ac40-ebecb5d8eaf6"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "      Name  Age         City\n",
              "0    Alice   24     New York\n",
              "1      Bob   27  Los Angeles\n",
              "2  Charlie   22      Chicago\n",
              "3    David   32      Houston"
            ],
            "text/html": [
              "\n",
              "  <div id=\"df-fb188530-bea2-478a-a393-61f6c3dac256\" class=\"colab-df-container\">\n",
              "    <div>\n",
              "<style scoped>\n",
              "    .dataframe tbody tr th:only-of-type {\n",
              "        vertical-align: middle;\n",
              "    }\n",
              "\n",
              "    .dataframe tbody tr th {\n",
              "        vertical-align: top;\n",
              "    }\n",
              "\n",
              "    .dataframe thead th {\n",
              "        text-align: right;\n",
              "    }\n",
              "</style>\n",
              "<table border=\"1\" class=\"dataframe\">\n",
              "  <thead>\n",
              "    <tr style=\"text-align: right;\">\n",
              "      <th></th>\n",
              "      <th>Name</th>\n",
              "      <th>Age</th>\n",
              "      <th>City</th>\n",
              "    </tr>\n",
              "  </thead>\n",
              "  <tbody>\n",
              "    <tr>\n",
              "      <th>0</th>\n",
              "      <td>Alice</td>\n",
              "      <td>24</td>\n",
              "      <td>New York</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>1</th>\n",
              "      <td>Bob</td>\n",
              "      <td>27</td>\n",
              "      <td>Los Angeles</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>2</th>\n",
              "      <td>Charlie</td>\n",
              "      <td>22</td>\n",
              "      <td>Chicago</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>3</th>\n",
              "      <td>David</td>\n",
              "      <td>32</td>\n",
              "      <td>Houston</td>\n",
              "    </tr>\n",
              "  </tbody>\n",
              "</table>\n",
              "</div>\n",
              "    <div class=\"colab-df-buttons\">\n",
              "\n",
              "  <div class=\"colab-df-container\">\n",
              "    <button class=\"colab-df-convert\" onclick=\"convertToInteractive('df-fb188530-bea2-478a-a393-61f6c3dac256')\"\n",
              "            title=\"Convert this dataframe to an interactive table.\"\n",
              "            style=\"display:none;\">\n",
              "\n",
              "  <svg xmlns=\"http://www.w3.org/2000/svg\" height=\"24px\" viewBox=\"0 -960 960 960\">\n",
              "    <path d=\"M120-120v-720h720v720H120Zm60-500h600v-160H180v160Zm220 220h160v-160H400v160Zm0 220h160v-160H400v160ZM180-400h160v-160H180v160Zm440 0h160v-160H620v160ZM180-180h160v-160H180v160Zm440 0h160v-160H620v160Z\"/>\n",
              "  </svg>\n",
              "    </button>\n",
              "\n",
              "  <style>\n",
              "    .colab-df-container {\n",
              "      display:flex;\n",
              "      gap: 12px;\n",
              "    }\n",
              "\n",
              "    .colab-df-convert {\n",
              "      background-color: #E8F0FE;\n",
              "      border: none;\n",
              "      border-radius: 50%;\n",
              "      cursor: pointer;\n",
              "      display: none;\n",
              "      fill: #1967D2;\n",
              "      height: 32px;\n",
              "      padding: 0 0 0 0;\n",
              "      width: 32px;\n",
              "    }\n",
              "\n",
              "    .colab-df-convert:hover {\n",
              "      background-color: #E2EBFA;\n",
              "      box-shadow: 0px 1px 2px rgba(60, 64, 67, 0.3), 0px 1px 3px 1px rgba(60, 64, 67, 0.15);\n",
              "      fill: #174EA6;\n",
              "    }\n",
              "\n",
              "    .colab-df-buttons div {\n",
              "      margin-bottom: 4px;\n",
              "    }\n",
              "\n",
              "    [theme=dark] .colab-df-convert {\n",
              "      background-color: #3B4455;\n",
              "      fill: #D2E3FC;\n",
              "    }\n",
              "\n",
              "    [theme=dark] .colab-df-convert:hover {\n",
              "      background-color: #434B5C;\n",
              "      box-shadow: 0px 1px 3px 1px rgba(0, 0, 0, 0.15);\n",
              "      filter: drop-shadow(0px 1px 2px rgba(0, 0, 0, 0.3));\n",
              "      fill: #FFFFFF;\n",
              "    }\n",
              "  </style>\n",
              "\n",
              "    <script>\n",
              "      const buttonEl =\n",
              "        document.querySelector('#df-fb188530-bea2-478a-a393-61f6c3dac256 button.colab-df-convert');\n",
              "      buttonEl.style.display =\n",
              "        google.colab.kernel.accessAllowed ? 'block' : 'none';\n",
              "\n",
              "      async function convertToInteractive(key) {\n",
              "        const element = document.querySelector('#df-fb188530-bea2-478a-a393-61f6c3dac256');\n",
              "        const dataTable =\n",
              "          await google.colab.kernel.invokeFunction('convertToInteractive',\n",
              "                                                    [key], {});\n",
              "        if (!dataTable) return;\n",
              "\n",
              "        const docLinkHtml = 'Like what you see? Visit the ' +\n",
              "          '<a target=\"_blank\" href=https://colab.research.google.com/notebooks/data_table.ipynb>data table notebook</a>'\n",
              "          + ' to learn more about interactive tables.';\n",
              "        element.innerHTML = '';\n",
              "        dataTable['output_type'] = 'display_data';\n",
              "        await google.colab.output.renderOutput(dataTable, element);\n",
              "        const docLink = document.createElement('div');\n",
              "        docLink.innerHTML = docLinkHtml;\n",
              "        element.appendChild(docLink);\n",
              "      }\n",
              "    </script>\n",
              "  </div>\n",
              "\n",
              "\n",
              "<div id=\"df-ba7d9ca4-0f2c-46fd-b272-f52aae3f873b\">\n",
              "  <button class=\"colab-df-quickchart\" onclick=\"quickchart('df-ba7d9ca4-0f2c-46fd-b272-f52aae3f873b')\"\n",
              "            title=\"Suggest charts\"\n",
              "            style=\"display:none;\">\n",
              "\n",
              "<svg xmlns=\"http://www.w3.org/2000/svg\" height=\"24px\"viewBox=\"0 0 24 24\"\n",
              "     width=\"24px\">\n",
              "    <g>\n",
              "        <path d=\"M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zM9 17H7v-7h2v7zm4 0h-2V7h2v10zm4 0h-2v-4h2v4z\"/>\n",
              "    </g>\n",
              "</svg>\n",
              "  </button>\n",
              "\n",
              "<style>\n",
              "  .colab-df-quickchart {\n",
              "      --bg-color: #E8F0FE;\n",
              "      --fill-color: #1967D2;\n",
              "      --hover-bg-color: #E2EBFA;\n",
              "      --hover-fill-color: #174EA6;\n",
              "      --disabled-fill-color: #AAA;\n",
              "      --disabled-bg-color: #DDD;\n",
              "  }\n",
              "\n",
              "  [theme=dark] .colab-df-quickchart {\n",
              "      --bg-color: #3B4455;\n",
              "      --fill-color: #D2E3FC;\n",
              "      --hover-bg-color: #434B5C;\n",
              "      --hover-fill-color: #FFFFFF;\n",
              "      --disabled-bg-color: #3B4455;\n",
              "      --disabled-fill-color: #666;\n",
              "  }\n",
              "\n",
              "  .colab-df-quickchart {\n",
              "    background-color: var(--bg-color);\n",
              "    border: none;\n",
              "    border-radius: 50%;\n",
              "    cursor: pointer;\n",
              "    display: none;\n",
              "    fill: var(--fill-color);\n",
              "    height: 32px;\n",
              "    padding: 0;\n",
              "    width: 32px;\n",
              "  }\n",
              "\n",
              "  .colab-df-quickchart:hover {\n",
              "    background-color: var(--hover-bg-color);\n",
              "    box-shadow: 0 1px 2px rgba(60, 64, 67, 0.3), 0 1px 3px 1px rgba(60, 64, 67, 0.15);\n",
              "    fill: var(--button-hover-fill-color);\n",
              "  }\n",
              "\n",
              "  .colab-df-quickchart-complete:disabled,\n",
              "  .colab-df-quickchart-complete:disabled:hover {\n",
              "    background-color: var(--disabled-bg-color);\n",
              "    fill: var(--disabled-fill-color);\n",
              "    box-shadow: none;\n",
              "  }\n",
              "\n",
              "  .colab-df-spinner {\n",
              "    border: 2px solid var(--fill-color);\n",
              "    border-color: transparent;\n",
              "    border-bottom-color: var(--fill-color);\n",
              "    animation:\n",
              "      spin 1s steps(1) infinite;\n",
              "  }\n",
              "\n",
              "  @keyframes spin {\n",
              "    0% {\n",
              "      border-color: transparent;\n",
              "      border-bottom-color: var(--fill-color);\n",
              "      border-left-color: var(--fill-color);\n",
              "    }\n",
              "    20% {\n",
              "      border-color: transparent;\n",
              "      border-left-color: var(--fill-color);\n",
              "      border-top-color: var(--fill-color);\n",
              "    }\n",
              "    30% {\n",
              "      border-color: transparent;\n",
              "      border-left-color: var(--fill-color);\n",
              "      border-top-color: var(--fill-color);\n",
              "      border-right-color: var(--fill-color);\n",
              "    }\n",
              "    40% {\n",
              "      border-color: transparent;\n",
              "      border-right-color: var(--fill-color);\n",
              "      border-top-color: var(--fill-color);\n",
              "    }\n",
              "    60% {\n",
              "      border-color: transparent;\n",
              "      border-right-color: var(--fill-color);\n",
              "    }\n",
              "    80% {\n",
              "      border-color: transparent;\n",
              "      border-right-color: var(--fill-color);\n",
              "      border-bottom-color: var(--fill-color);\n",
              "    }\n",
              "    90% {\n",
              "      border-color: transparent;\n",
              "      border-bottom-color: var(--fill-color);\n",
              "    }\n",
              "  }\n",
              "</style>\n",
              "\n",
              "  <script>\n",
              "    async function quickchart(key) {\n",
              "      const quickchartButtonEl =\n",
              "        document.querySelector('#' + key + ' button');\n",
              "      quickchartButtonEl.disabled = true;  // To prevent multiple clicks.\n",
              "      quickchartButtonEl.classList.add('colab-df-spinner');\n",
              "      try {\n",
              "        const charts = await google.colab.kernel.invokeFunction(\n",
              "            'suggestCharts', [key], {});\n",
              "      } catch (error) {\n",
              "        console.error('Error during call to suggestCharts:', error);\n",
              "      }\n",
              "      quickchartButtonEl.classList.remove('colab-df-spinner');\n",
              "      quickchartButtonEl.classList.add('colab-df-quickchart-complete');\n",
              "    }\n",
              "    (() => {\n",
              "      let quickchartButtonEl =\n",
              "        document.querySelector('#df-ba7d9ca4-0f2c-46fd-b272-f52aae3f873b button');\n",
              "      quickchartButtonEl.style.display =\n",
              "        google.colab.kernel.accessAllowed ? 'block' : 'none';\n",
              "    })();\n",
              "  </script>\n",
              "</div>\n",
              "\n",
              "  <div id=\"id_390327d7-db78-4447-b806-277aa59fb2b0\">\n",
              "    <style>\n",
              "      .colab-df-generate {\n",
              "        background-color: #E8F0FE;\n",
              "        border: none;\n",
              "        border-radius: 50%;\n",
              "        cursor: pointer;\n",
              "        display: none;\n",
              "        fill: #1967D2;\n",
              "        height: 32px;\n",
              "        padding: 0 0 0 0;\n",
              "        width: 32px;\n",
              "      }\n",
              "\n",
              "      .colab-df-generate:hover {\n",
              "        background-color: #E2EBFA;\n",
              "        box-shadow: 0px 1px 2px rgba(60, 64, 67, 0.3), 0px 1px 3px 1px rgba(60, 64, 67, 0.15);\n",
              "        fill: #174EA6;\n",
              "      }\n",
              "\n",
              "      [theme=dark] .colab-df-generate {\n",
              "        background-color: #3B4455;\n",
              "        fill: #D2E3FC;\n",
              "      }\n",
              "\n",
              "      [theme=dark] .colab-df-generate:hover {\n",
              "        background-color: #434B5C;\n",
              "        box-shadow: 0px 1px 3px 1px rgba(0, 0, 0, 0.15);\n",
              "        filter: drop-shadow(0px 1px 2px rgba(0, 0, 0, 0.3));\n",
              "        fill: #FFFFFF;\n",
              "      }\n",
              "    </style>\n",
              "    <button class=\"colab-df-generate\" onclick=\"generateWithVariable('df')\"\n",
              "            title=\"Generate code using this dataframe.\"\n",
              "            style=\"display:none;\">\n",
              "\n",
              "  <svg xmlns=\"http://www.w3.org/2000/svg\" height=\"24px\"viewBox=\"0 0 24 24\"\n",
              "       width=\"24px\">\n",
              "    <path d=\"M7,19H8.4L18.45,9,17,7.55,7,17.6ZM5,21V16.75L18.45,3.32a2,2,0,0,1,2.83,0l1.4,1.43a1.91,1.91,0,0,1,.58,1.4,1.91,1.91,0,0,1-.58,1.4L9.25,21ZM18.45,9,17,7.55Zm-12,3A5.31,5.31,0,0,0,4.9,8.1,5.31,5.31,0,0,0,1,6.5,5.31,5.31,0,0,0,4.9,4.9,5.31,5.31,0,0,0,6.5,1,5.31,5.31,0,0,0,8.1,4.9,5.31,5.31,0,0,0,12,6.5,5.46,5.46,0,0,0,6.5,12Z\"/>\n",
              "  </svg>\n",
              "    </button>\n",
              "    <script>\n",
              "      (() => {\n",
              "      const buttonEl =\n",
              "        document.querySelector('#id_390327d7-db78-4447-b806-277aa59fb2b0 button.colab-df-generate');\n",
              "      buttonEl.style.display =\n",
              "        google.colab.kernel.accessAllowed ? 'block' : 'none';\n",
              "\n",
              "      buttonEl.onclick = () => {\n",
              "        google.colab.notebook.generateWithVariable('df');\n",
              "      }\n",
              "      })();\n",
              "    </script>\n",
              "  </div>\n",
              "\n",
              "    </div>\n",
              "  </div>\n"
            ],
            "application/vnd.google.colaboratory.intrinsic+json": {
              "type": "dataframe",
              "variable_name": "df",
              "summary": "{\n  \"name\": \"df\",\n  \"rows\": 4,\n  \"fields\": [\n    {\n      \"column\": \"Name\",\n      \"properties\": {\n        \"dtype\": \"string\",\n        \"num_unique_values\": 4,\n        \"samples\": [\n          \"Bob\",\n          \"David\",\n          \"Alice\"\n        ],\n        \"semantic_type\": \"\",\n        \"description\": \"\"\n      }\n    },\n    {\n      \"column\": \"Age\",\n      \"properties\": {\n        \"dtype\": \"number\",\n        \"std\": 4,\n        \"min\": 22,\n        \"max\": 32,\n        \"num_unique_values\": 4,\n        \"samples\": [\n          27,\n          32,\n          24\n        ],\n        \"semantic_type\": \"\",\n        \"description\": \"\"\n      }\n    },\n    {\n      \"column\": \"City\",\n      \"properties\": {\n        \"dtype\": \"string\",\n        \"num_unique_values\": 4,\n        \"samples\": [\n          \"Los Angeles\",\n          \"Houston\",\n          \"New York\"\n        ],\n        \"semantic_type\": \"\",\n        \"description\": \"\"\n      }\n    }\n  ]\n}"
            }
          },
          "metadata": {},
          "execution_count": 98
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "You can access individual columns using the column name, multiple columns by passing a list of column names, and specific rows using the .iloc[] method or by applying conditions."
      ],
      "metadata": {
        "id": "znEFC8PP1H7A"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "print(df['Name'])\n",
        "print(df[['Name', 'City']])\n",
        "print(df.iloc[0])\n",
        "print(df[df['Age'] > 25])"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "75dvatBT1J6b",
        "outputId": "891191bb-5920-442b-ff3b-7edc0b3f130a"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0      Alice\n",
            "1        Bob\n",
            "2    Charlie\n",
            "3      David\n",
            "Name: Name, dtype: object\n",
            "      Name         City\n",
            "0    Alice     New York\n",
            "1      Bob  Los Angeles\n",
            "2  Charlie      Chicago\n",
            "3    David      Houston\n",
            "Name       Alice\n",
            "Age           24\n",
            "City    New York\n",
            "Name: 0, dtype: object\n",
            "    Name  Age         City\n",
            "1    Bob   27  Los Angeles\n",
            "3  David   32      Houston\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Pandas allows for easy manipulation of DataFrames. In this example, we add a new column Salary to the DataFrame. We then calculate the mean age of the group using the .mean() method, which can be applied directly to a column."
      ],
      "metadata": {
        "id": "-NpGUFLV1R9U"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "df['Salary'] = [70000, 80000, 60000, 90000]\n",
        "\n",
        "mean_age = df['Age'].mean()\n",
        "\n",
        "print(\"DataFrame after adding 'Salary' column:\")\n",
        "print(df)\n",
        "\n",
        "print(f\"\\nMean Age of the group: {mean_age:.2f} years\") # here .2f rounds off decimal place to 2 digits"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "GcO_m-Ot1Tyz",
        "outputId": "288ec6bb-9ed3-4490-a64d-9a26cd143a61"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "DataFrame after adding 'Salary' column:\n",
            "      Name  Age         City  Salary\n",
            "0    Alice   24     New York   70000\n",
            "1      Bob   27  Los Angeles   80000\n",
            "2  Charlie   22      Chicago   60000\n",
            "3    David   32      Houston   90000\n",
            "\n",
            "Mean Age of the group: 26.25 years\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Handling missing data is a common task in data analysis. This cell demonstrates how to introduce missing values (NaN) in a DataFrame and how to handle them using the .fillna() method. In this case, we fill the missing age with the mean age of the group."
      ],
      "metadata": {
        "id": "RRPAQV7D1by3"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "df.loc[2, 'Age'] = None\n",
        "\n",
        "print(\"DataFrame with missing value:\")\n",
        "print(df)\n",
        "\n",
        "df_filled = df.fillna(df['Age'].mean())\n",
        "\n",
        "print(\"\\nDataFrame after filling missing values with mean age:\")\n",
        "print(df_filled)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "VfG6xV2R1pcq",
        "outputId": "9da4d837-74fc-47ae-971d-be4d504f01aa"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "DataFrame with missing value:\n",
            "      Name   Age         City  Salary\n",
            "0    Alice  24.0     New York   70000\n",
            "1      Bob  27.0  Los Angeles   80000\n",
            "2  Charlie   NaN      Chicago   60000\n",
            "3    David  32.0      Houston   90000\n",
            "\n",
            "DataFrame after filling missing values with mean age:\n",
            "      Name        Age         City  Salary\n",
            "0    Alice  24.000000     New York   70000\n",
            "1      Bob  27.000000  Los Angeles   80000\n",
            "2  Charlie  27.666667      Chicago   60000\n",
            "3    David  32.000000      Houston   90000\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Aggregation is another powerful feature of pandas. In this cell, we group the DataFrame by the City column and calculate the mean of the Age and Salary columns for each city. The .groupby() and .agg() methods are used for this purpose."
      ],
      "metadata": {
        "id": "kLAfUEhL1wzl"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "grouped = df.groupby('City').agg({'Age': 'mean', 'Salary': 'mean'})\n",
        "print(\"Mean Age and Salary by City:\")\n",
        "print(grouped)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "YfNWlygv1yOH",
        "outputId": "d84cdbc2-0fa7-49da-ab6c-cc56f4fd0ec2"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Mean Age and Salary by City:\n",
            "              Age   Salary\n",
            "City                      \n",
            "Chicago       NaN  60000.0\n",
            "Houston      32.0  90000.0\n",
            "Los Angeles  27.0  80000.0\n",
            "New York     24.0  70000.0\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Flask"
      ],
      "metadata": {
        "id": "BjAiJOzk2EPA"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Flask is a lightweight web framework for Python, designed to make it easy to build web applications. It is known for its simplicity and flexibility, allowing developers to create web apps with minimal overhead. Flask follows the WSGI (Web Server Gateway Interface) standard and is based on Werkzeug and Jinja2.\n"
      ],
      "metadata": {
        "id": "t6AYBtbl2OCH"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "!pip install flask"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "xycwI0822QlH",
        "outputId": "86ed2b7b-c935-4449-8213-85ba5f58a3e5"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Requirement already satisfied: flask in /usr/local/lib/python3.10/dist-packages (2.2.5)\n",
            "Requirement already satisfied: Werkzeug>=2.2.2 in /usr/local/lib/python3.10/dist-packages (from flask) (3.0.3)\n",
            "Requirement already satisfied: Jinja2>=3.0 in /usr/local/lib/python3.10/dist-packages (from flask) (3.1.4)\n",
            "Requirement already satisfied: itsdangerous>=2.0 in /usr/local/lib/python3.10/dist-packages (from flask) (2.2.0)\n",
            "Requirement already satisfied: click>=8.0 in /usr/local/lib/python3.10/dist-packages (from flask) (8.1.7)\n",
            "Requirement already satisfied: MarkupSafe>=2.0 in /usr/local/lib/python3.10/dist-packages (from Jinja2>=3.0->flask) (2.1.5)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "We create a basic Flask application. The Flask class is used to create an app instance, and we define a route using the @app.route decorator. This route maps the URL path '/' (home page) to the home() function, which returns a simple string message.\n",
        "\n",
        "NOTE: YOU HAVE TO RUN ALL THE FOLLOWING CODE IN LOCAL (VSCODE)"
      ],
      "metadata": {
        "id": "669k-vMp2XnU"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "from flask import Flask\n",
        "\n",
        "app = Flask(__name__)\n",
        "\n",
        "@app.route('/')\n",
        "def home():\n",
        "    return \"Welcome to Flask!\"\n",
        "\n",
        "@app.route('/about')\n",
        "def about():\n",
        "    return \"This is the about page.\"\n",
        "\n",
        "\n",
        "@app.route('/user/<name>') # A route with a dynamic URL parameter\n",
        "def user(name):\n",
        "    return f\"Hello, {name}!\"\n",
        "\n",
        "if __name__ == \"__main__\":\n",
        "    app.run(debug=True)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "WI6YcsSc2an-",
        "outputId": "2ec1d881-2f70-4f49-af4d-c3d106ca1a14"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            " * Serving Flask app '__main__'\n",
            " * Debug mode: on\n"
          ]
        },
        {
          "output_type": "stream",
          "name": "stderr",
          "text": [
            "INFO:werkzeug:\u001b[31m\u001b[1mWARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.\u001b[0m\n",
            " * Running on http://127.0.0.1:5000\n",
            "INFO:werkzeug:\u001b[33mPress CTRL+C to quit\u001b[0m\n",
            "INFO:werkzeug: * Restarting with stat\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Flask allows you to handle different HTTP methods (GET, POST, etc.). In this example, the /submit route handles both GET and POST requests. If the request method is POST, it processes the form data and returns a response; otherwise, it displays an HTML form."
      ],
      "metadata": {
        "id": "D6V7U0ZZ3E0t"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "from flask import request\n",
        "\n",
        "@app.route('/submit', methods=['GET', 'POST'])\n",
        "def submit():\n",
        "    if request.method == 'POST':\n",
        "        name = request.form.get('name')\n",
        "        return f\"Form submitted! Hello, {name}!\"\n",
        "    return '''\n",
        "        <form method=\"post\">\n",
        "            Name: <input type=\"text\" name=\"name\">\n",
        "            <input type=\"submit\">\n",
        "        </form>\n",
        "    '''"
      ],
      "metadata": {
        "id": "dar15ZRn3GtD"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Flask uses the Jinja2 template engine to render HTML templates. In this example, we use the render_template() function to render an HTML file named index.html."
      ],
      "metadata": {
        "id": "gulArvZ_3NxP"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "from flask import render_template\n",
        "\n",
        "# write a simple 'index.html' file in a 'templates' folder\n",
        "@app.route('/template')\n",
        "def template():\n",
        "    return render_template('index.html')"
      ],
      "metadata": {
        "id": "S3Hyi2IR3OJn"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Flask can easily handle JSON data using the jsonify() function. In this cell, the /data route returns a JSON response containing some user data. This is particularly useful when building APIs."
      ],
      "metadata": {
        "id": "2GQyznNX3WeJ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "from flask import jsonify\n",
        "\n",
        "@app.route('/data')\n",
        "def data():\n",
        "    response_data = {'name': 'Alice', 'age': 24, 'city': 'New York'}\n",
        "    return jsonify(response_data)"
      ],
      "metadata": {
        "id": "s_-KO3Mm3WCb"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "This example demonstrates how to create a RESTful API endpoint in Flask. The /api/user/<int:id> route takes an integer ID as a parameter and returns the corresponding user’s name in JSON format."
      ],
      "metadata": {
        "id": "lPOhgnC43dwz"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "@app.route('/api/user/<int:id>', methods=['GET'])\n",
        "def get_user(id):\n",
        "    users = {1: 'Alice', 2: 'Bob', 3: 'Charlie'}\n",
        "    user = users.get(id, 'User not found')\n",
        "    return jsonify({'id': id, 'name': user})"
      ],
      "metadata": {
        "id": "EoiV3tLl3eX8"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "**Exercise Time**\n",
        "\n",
        "Objective:\n",
        "\n",
        "Create a simple Flask application that integrates with a pre-trained model from Hugging Face. The application will allow users to input text and receive a response generated by the model.\n",
        "\n",
        "Exercise Requirements:\n",
        "\n",
        "Set up a basic Flask application.\n",
        "Create a single route (/predict) that accepts POST requests.\n",
        "The route should accept user input (text) and pass it to a Hugging Face model for processing.\n",
        "Return the model's output to the user.\n",
        "\n",
        "Use the Hugging Face 'transformers' library to load a pre-trained model.\n",
        "For simplicity, use a text generation model like 'distilgpt2'."
      ],
      "metadata": {
        "id": "hFEOn6RR4kYD"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Study Resources"
      ],
      "metadata": {
        "id": "DVQ5ll_J5Inl"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Data analytics:\n",
        "\n",
        "[Python Libraries In-Depth](https://www.udemy.com/course/data-analytics-in-python/)\n",
        "\n",
        "Testing:\n",
        "\n",
        "[RealPython](https://realpython.com/python-doctest/)\n",
        "\n",
        "[PyTest](https://docs.pytest.org/en/stable/contents.html)\n",
        "\n",
        "Backend:\n",
        "\n",
        "[Django](https://www.djangoproject.com/)\n",
        "\n",
        "[DjangoGirls](https://tutorial.djangogirls.org/en/)\n",
        "\n",
        "[FastAPI](https://fastapi.tiangolo.com/)\n",
        "\n",
        "Networking using Python:\n",
        "\n",
        "[Network Protocols and Web Sockets](https://medium.com/@AlexanderObregon/python-for-network-programming-a-beginners-overview-e9379cc44479#:~:text=The%20Role%20of%20Python%20in,client%20and%20http.)\n",
        "\n",
        "GUI:\n",
        "\n",
        "[RealPython](https://realpython.com/python-gui-tkinter/)\n",
        "\n",
        "[Tkinter](https://docs.codio.com/instructors/setupcourses/resources/resourcetools/tkinter.html)\n",
        "\n",
        "*Advanced*\n",
        "\n",
        "Automation:\n",
        "\n",
        "[Projects based on Selenium or BeautifulSoup](https://www.geeksforgeeks.org/python-automation/)\n",
        "\n",
        "Artificial Intelligence:\n",
        "\n",
        "[Language](https://www.analyticsvidhya.com/blog/2022/05/a-complete-guide-on-chatbot-development-using-python/)\n",
        "\n",
        "[Videos and Images](https://www.analyticsvidhya.com/blog/2023/09/image-generation-using-stable-diffusion/)\n",
        "\n",
        "\n",
        "Courses:\n",
        "\n",
        "[cs50p](https://cs50.harvard.edu/python/2022/) you can skip a few lectures (I would recommend to start watching lectures from week 5) but do all the exercises\n",
        "\n",
        "[GooglePythonClass](https://www.youtube.com/playlist?list=PLC8825D0450647509) this is a video course if that helps"
      ],
      "metadata": {
        "id": "s8WJTf2S5PjJ"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Final Project (OPTIONAL)"
      ],
      "metadata": {
        "id": "8tm2u49a_HoN"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## **Expense Tracker with Data Analysis and Visualization**\n",
        "\n",
        "### **Project Overview:**\n",
        "\n",
        "Create a command-line or web-based expense tracker that allows users to record, analyze, and visualize their expenses. This project will incorporate various Python concepts, including loops, conditionals, data structures, functions, error handling, OOP, file I/O, and data analysis with NumPy and Pandas.\n",
        "\n",
        "### **Project Requirements:**\n",
        "\n",
        "**Data Input and Storage:**\n",
        "\n",
        "Allow users to input their daily expenses, including date, category (e.g., food, transportation), and amount.\n",
        "Store the expenses in a file (e.g., CSV) or in-memory using lists, tuples, or dictionaries.\n",
        "\n",
        "**Data Processing:**\n",
        "\n",
        "Implement functions to load, save, and process the expense data.\n",
        "Use loops, if-else statements, and functions to filter and categorize expenses.\n",
        "\n",
        "**String Manipulation and Regular Expressions:**\n",
        "\n",
        "Parse and validate user input, such as dates and categories, using string manipulation and regular expressions.\n",
        "Ensure that dates are in the correct format and categories match predefined options.\n",
        "\n",
        "**Error Handling:**\n",
        "\n",
        "Implement try-except blocks to handle possible errors (e.g., invalid input, file not found).\n",
        "\n",
        "**Object-Oriented Programming:**\n",
        "\n",
        "Design classes to represent an Expense and an ExpenseTracker with methods for adding, deleting, and summarizing expenses.\n",
        "Use decorators for any additional functionality (e.g., logging).\n",
        "\n",
        "**Data Analysis with NumPy and Pandas:**\n",
        "\n",
        "Convert the expense data into a Pandas DataFrame for easy manipulation and analysis.\n",
        "Use NumPy for numerical operations, such as calculating total expenses, average spending, and category-wise breakdowns.\n",
        "Perform basic regression analysis to predict future expenses based on historical data.\n",
        "\n",
        "**Visualization:**\n",
        "\n",
        "Create visualizations (e.g., bar charts, pie charts) to display the distribution of expenses by category or over time.\n",
        "Use Pandas plotting functions or Matplotlib for visualization.\n",
        "\n",
        "**Flask Integration (Optional):**\n",
        "\n",
        "Optionally, build a simple Flask app with routes for inputting expenses, viewing summaries, and displaying visualizations.\n",
        "Use Flask to provide a web-based interface for the expense tracker.\n",
        "\n",
        "### **Step-by-Step Implementation:**\n",
        "\n",
        "**Set Up the Expense Tracker:**\n",
        "\n",
        "Create classes for Expense (attributes: date, category, amount) and ExpenseTracker (methods: add_expense, delete_expense, summarize_expenses).\n",
        "Implement functions to read/write expenses from/to a file.\n",
        "\n",
        "**Data Input and Validation:**\n",
        "\n",
        "Implement a command-line interface (CLI) or web form to input expenses.\n",
        "Use regular expressions to validate the date format and ensure categories are correct.\n",
        "\n",
        "**Expense Analysis:**\n",
        "\n",
        "Write functions to calculate total expenses, monthly summaries, and category-wise distributions.\n",
        "Use NumPy and Pandas to perform data analysis and create summaries.\n",
        "\n",
        "**Visualization:**\n",
        "\n",
        "Generate visualizations to help users understand their spending habits.\n",
        "Create bar charts showing monthly expenses or pie charts showing category distributions.\n",
        "\n",
        "**Error Handling and Scope Management:**\n",
        "\n",
        "Ensure all user inputs are validated and handled gracefully using try-except.\n",
        "Keep data encapsulated within classes and methods, and manage variable scope effectively.\n",
        "\n",
        "**Flask Integration (Optional):**\n",
        "\n",
        "If creating a web-based app, build a simple Flask application with routes for adding expenses and viewing summaries.\n",
        "Display visualizations directly in the web interface using Flask templates.\n",
        "\n",
        "### **Project Outcome:**\n",
        "\n",
        "By the end of this project, you will have an expense tracker that allows users to record and analyze their expenses. This project will help you practice Python's core concepts and provide a practical tool for managing personal finances.\n",
        "\n",
        "**Bonus Features:**\n",
        "\n",
        "Add a feature to export expense summaries as CSV or PDF.\n",
        "Include advanced filtering options, like filtering by date range or category.\n",
        "Extend the app to allow multiple users with separate expense tracking."
      ],
      "metadata": {
        "id": "Q_6JxhzB_J7Q"
      }
    }
  ]
}