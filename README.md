# Request Response Cycle, APIs, and Postman Lab

You will be working with a free API of your choice for this lab.

## Getting Started

1. Choose an API with no auth and no CORS from the following list. It _should not_ be one that you've already seen or worked on in class.
   - [Public APIs](https://github.com/public-apis/public-apis)
1. Choose an API not covered in your readings, class, or other assignments. The API should be new to you.
1. Write your answers in this README.md file. Do not delete the questions. Write your answers after the `>`. If you need to write more than one paragraph, add more `>`.
1. Take the time to read back the work, and edit what you've written so that your answers are clear and anyone reading it can easily understand what you've written.

## Instructions

Do your best to answer the questions with specific details. Writing about code clearly and thoroughly is a critical skill to practice.

- Which one did you choose? Provide the name and base URL.

> https://color.serialif.com/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The purpose of this API is to get a requested color, its complementary and its grayscale in different formats and the black or white text corresponding to each color according to its brightness.

- What is the URL of the documentation?

> https://color.serialif.com/

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> https://color.serialif.com/aquamarine

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json
{
    "status": "success",
    "base": {
        "keyword": "aquamarine",
        "hex": {
            "value": "#7fffd4",
            "composition": {
                "red": "7f",
                "green": "ff",
                "blue": "d4"
            }
        },
        "rgb": {
            "value": "rgb(127, 255, 212)",
            "composition": {
                "red": 127,
                "green": 255,
                "blue": 212
            }
        },
        "hsl": {
            "value": "hsl(160, 100%, 75%)",
            "composition": {
                "hue": 160,
                "saturation": 100,
                "lightness": 75
            }
        },
        "hsl_raw": {
            "value": "hsl(159.84375, 100%, 74.90196%)",
            "composition": {
                "hue": 159.84375,
                "saturation": 100,
                "lightness": 74.90196
            }
        }
    },
    "base_without_alpha": {
        "keyword": "aquamarine",
        "hex": {
            "value": "#7fffd4",
            "composition": {
                "red": "7f",
                "green": "ff",
                "blue": "d4"
            }
        },
        "rgb": {
            "value": "rgb(127, 255, 212)",
            "composition": {
                "red": 127,
                "green": 255,
                "blue": 212
            }
        },
        "hsl": {
            "value": "hsl(160, 100%, 75%)",
            "composition": {
                "hue": 160,
                "saturation": 100,
                "lightness": 75
            }
        },
        "hsl_raw": {
            "value": "hsl(159.84375, 100%, 74.90196%)",
            "composition": {
                "hue": 159.84375,
                "saturation": 100,
                "lightness": 74.90196
            }
        }
    },
    "base_without_alpha_contrasted_text": {
        "keyword": "black",
        "hex": {
            "value": "#000000",
            "composition": {
                "red": "00",
                "green": "00",
                "blue": "00"
            }
        },
        "rgb": {
            "value": "rgb(0, 0, 0)",
            "composition": {
                "red": 0,
                "green": 0,
                "blue": 0
            }
        },
        "hsl": {
            "value": "hsl(0, 0%, 0%)",
            "composition": {
                "hue": 0,
                "saturation": 0,
                "lightness": 0
            }
        },
        "hsl_raw": {
            "value": "hsl(0, 0%, 0%)",
            "composition": {
                "hue": 0,
                "saturation": 0,
                "lightness": 0
            }
        }
    },
    "complementary": {
        "keyword": "",
        "hex": {
            "value": "#80002b",
            "composition": {
                "red": "80",
                "green": "00",
                "blue": "2b"
            }
        },
        "rgb": {
            "value": "rgb(128, 0, 43)",
            "composition": {
                "red": 128,
                "green": 0,
                "blue": 43
            }
        },
        "hsl": {
            "value": "hsl(340, 100%, 25%)",
            "composition": {
                "hue": 340,
                "saturation": 100,
                "lightness": 25
            }
        },
        "hsl_raw": {
            "value": "hsl(339.84375, 100%, 25.09804%)",
            "composition": {
                "hue": 339.84375,
                "saturation": 100,
                "lightness": 25.09804
            }
        }
    },
    "complementary_without_alpha": {
        "keyword": "",
        "hex": {
            "value": "#80002b",
            "composition": {
                "red": "80",
                "green": "00",
                "blue": "2b"
            }
        },
        "rgb": {
            "value": "rgb(128, 0, 43)",
            "composition": {
                "red": 128,
                "green": 0,
                "blue": 43
            }
        },
        "hsl": {
            "value": "hsl(340, 100%, 25%)",
            "composition": {
                "hue": 340,
                "saturation": 100,
                "lightness": 25
            }
        },
        "hsl_raw": {
            "value": "hsl(339.84375, 100%, 25.09804%)",
            "composition": {
                "hue": 339.84375,
                "saturation": 100,
                "lightness": 25.09804
            }
        }
    },
    "complementary_without_alpha_contrasted_text": {
        "keyword": "white",
        "hex": {
            "value": "#ffffff",
            "composition": {
                "red": "ff",
                "green": "ff",
                "blue": "ff"
            }
        },
        "rgb": {
            "value": "rgb(255, 255, 255)",
            "composition": {
                "red": 255,
                "green": 255,
                "blue": 255
            }
        },
        "hsl": {
            "value": "hsl(0, 0%, 100%)",
            "composition": {
                "hue": 0,
                "saturation": 0,
                "lightness": 100
            }
        },
        "hsl_raw": {
            "value": "hsl(0, 0%, 100%)",
            "composition": {
                "hue": 0,
                "saturation": 0,
                "lightness": 100
            }
        }
    },
    "grayscale": {
        "keyword": "",
        "hex": {
            "value": "#bfbfbf",
            "composition": {
                "red": "bf",
                "green": "bf",
                "blue": "bf"
            }
        },
        "rgb": {
            "value": "rgb(191, 191, 191)",
            "composition": {
                "red": 191,
                "green": 191,
                "blue": 191
            }
        },
        "hsl": {
            "value": "hsl(160, 0%, 75%)",
            "composition": {
                "hue": 160,
                "saturation": 0,
                "lightness": 75
            }
        },
        "hsl_raw": {
            "value": "hsl(159.84375, 0%, 74.90196%)",
            "composition": {
                "hue": 159.84375,
                "saturation": 0,
                "lightness": 74.90196
            }
        }
    },
    "grayscale_without_alpha": {
        "keyword": "",
        "hex": {
            "value": "#bfbfbf",
            "composition": {
                "red": "bf",
                "green": "bf",
                "blue": "bf"
            }
        },
        "rgb": {
            "value": "rgb(191, 191, 191)",
            "composition": {
                "red": 191,
                "green": 191,
                "blue": 191
            }
        },
        "hsl": {
            "value": "hsl(160, 0%, 75%)",
            "composition": {
                "hue": 160,
                "saturation": 0,
                "lightness": 75
            }
        },
        "hsl_raw": {
            "value": "hsl(159.84375, 0%, 74.90196%)",
            "composition": {
                "hue": 159.84375,
                "saturation": 0,
                "lightness": 74.90196
            }
        }
    },
    "grayscale_without_alpha_contrasted_text": {
        "keyword": "black",
        "hex": {
            "value": "#000000",
            "composition": {
                "red": "00",
                "green": "00",
                "blue": "00"
            }
        },
        "rgb": {
            "value": "rgb(0, 0, 0)",
            "composition": {
                "red": 0,
                "green": 0,
                "blue": 0
            }
        },
        "hsl": {
            "value": "hsl(0, 0%, 0%)",
            "composition": {
                "hue": 0,
                "saturation": 0,
                "lightness": 0
            }
        },
        "hsl_raw": {
            "value": "hsl(0, 0%, 0%)",
            "composition": {
                "hue": 0,
                "saturation": 0,
                "lightness": 0
            }
        }
    }
}

```

- What status code did you get back from your request? Why did you receive this status code?

> 200 OK. Received this status it's the standard response for successful HTTPS requests.

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json

> `Content-Length`: not available

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes Color values in various forms like hex and rgb. 

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that needs to have automatic references for color contrast values. 

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The documentation was I like that it was organized in one page and examples of use were displayed.

- What did you find challenging about the documentation? Cite specific examples.

> I found the documentation hard to understand as documentation because I was looking for it on another page and that I expected labeled as such. 

- Did the quality of the documentation impact your decision to use it?

> No because the information wouldn't be used for much more than just color alterations/suggestions. If I needed better quality from these recommendations it might in the future. 

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> Yes I switched. I was looking for something with immediate use and simplicity yet without much restrictions.

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle start when a client sends request to api endpoint. The request is processed and then returns a response containing data. 

- In your own words, describe what an API is.

> An API (Application Programming Interface) acts as a digital bridge, enabling seamless communication between software components through a request-response cycle, enhancing development efficiency and consistency.

- In your own words, describe the purpose of Postman.

> Postman is an application for API development, testing, and collaboration. 