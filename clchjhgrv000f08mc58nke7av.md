# Learn HTML:    HTML input elements

# "What are input elements:"

The input elements are nothing but we are taking input from users in the following list of ways:

* Text
    
* Number
    
* Checkbox
    
* Radio
    
* Colour
    
* Email
    
* Range
    
* Date
    
* Time
    
* Datetime-local
    
* tel
    
* Password
    
* Submit
    
* Button
    
* File
    
* Hidden
    
* Month
    
* week
    
* URL
    
* Reset
    

These are all types of inputs.

# "Input Syntax:"

we define input by using `<input type="text">` tag. The default type is text it has no end tag.

# "Definition of each input type"

### 1\. Text

The `<input type="text">` is used to take text as input from the user. We can also specify the "maxlength" attribute to take input of a certain length. The "value" attribute is used to define the default attribute.

![Text input looks like this.](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAa8AAAB1CAMAAADOZ57OAAAAh1BMVEX////+/v7z8/MAAABcXFyNjY3Jycn7+/v4+Pj29vbw8PDt7e2urq5xcXGrq6vd3d3T09PCwsJjY2OTk5N3d3ednZ21tbXU1NSjo6Po6OiPj49paWmCgoJ9fX1YWFji4uIoKCgzMzNISEghISE+Pj4WFhZPT08YGBg5OTkkJCQvLy8ODg5ERETT0PVfAAALZElEQVR4nO2d2WKqOhRAAxsIc5gHAXGq2tr//767E3BoT09b7SC5J+vBooawycqIYglRKBQKhUKhUCgUCoVCoVAoFAqFQqFQKP7nuPcO4Hbs05Z+xyh+nMpIEmMeVCUhcQbZnaNx2vlmnWpX78fMRSo2aNxA/t1RTYOhVLwCIPUDgJZEwRd90a+GRIPE1VcQXZ11H8DoK0re9vXl2O6ONlZjOGDbYgAhib7mq0i/GlLMVenxn2UbBR/sGZ0sFW/68hLphWmjMDjw+ryF5E9fV3VM7OHLHVELbw+g3uLzvvxx60Xsznz+1djujjYKG3zNwTj6yrMs5n/9IMkY/mVZ0+ZYPe08685dVdQGqYMl4aduFaSU9GvYtha2kS6r8G07DPsuFwdoZzOzJoXZeoRYbWDyobLrYlJ0XYEuzNIKCp6Opnto0zTNMBca5nVrEq9ruhn1lrBsi+GwdtokM5xReHmup4HPD2DPgix/5cvKkiAW7zVZ2jsNPHWhCIZamR5nbY+bdds0PC0tKrvK8AyrzPREFp0IyAnCHyz+q9FGYaI/dAFPU/hysWgMHM1IChZa7EkNvm0uHdLv0mIF1bh3tfBzWNf1Bp7WxjOmLzNoQkaCbdHCVosBtgAgpmq47WMBbzqNZFDEc16gJsyIluPxZgANwIKno/4Scj9cYWocVDcLAG/R2j7QvoNtONaU/aKudxsMFY/bLHjG9WPDrMNLXwX27ibGT7aGHoPlVbCpRB0kBsB8mcAaA4I5hmmS6ACbXbOHbLU1YEUJNZIiwNqLmSym1IlqozA4FH2xBEMffGVbLAIAZq+wc4qhICEwQhOdzDustgDDvDnijbKDjtQPEGNXiD5j7rJ4rIk9H0q8ZkMRYTeHI1u/80QxEn2Je8T8pQj3pyksqVUOCedcsI/H1HB3xmKL+5jreNhjR+3xgkwwCAseenwQz7BUw5e+AqxnJR6Cog/SxsTG3n7EAOwMNnhOBVYZZ7WkBGX3mDEUmrbCulsBFsoaY7S74pdUfIrRl4bNAJ4ayybCV73eJ0aCwZMoJk4mSn6PRvDN58TANjPU8xYMI9ljNXUXS4/gnE7HdBXWzR3uvYYAk59KiPSAafxntA41Ps2xlIUvC31h+Z57nTl4gy8s7BXhAe0K0lNMfRpYi5KwDWbDYIMtEraYBpVgVi989ZjFDBu9BoeU6BggJMfxrAGsHBnqcPyaxIudjbXtGV8/rDV+WhHZ7EQBTG5VcPJ1YOMr3JcFleshWGfLZMV9YQWGeY9lFoo3hvPeP4onOvdVE2c7+tIPiXjdfjl36fCtZUxwHOK+LNi98HWuxZe+DP6CCbDkw91FZvE+2x99EfQVC9+v5xt1t8x4p+4DPGAr18+1R/jq0BeOkY/Zk/DFs1qsbX68qN8F4ylMjLOvaBzLBl+teNfGU02J6JBovoZ9HY/tYDiP5YGXPKHaK1+wdYZEL3yVsC+fPeJuhC8Gj5/1pRU4ipWYujsGnR1iLPILX6FYeb3yFUFgl+JMrBXvK97y5WyWzN4+vPbFHlbDeV6/av9ZzuPXpa/ywIcDwsweh2MsKJ/EJam3UEXDpMAaFlnJMPHIPJ33hydf9JkP8kTPnJdrgy08YeFhf8jdRMf+MPrIV2QRN8DO9eyLTxBe+ophT1770p93OuG+7JBoLVaPt3zNMNTRF+8Pj75weOWTRzeYWgM7j19HX2JYN2BbetY6YvBc6wFUNG95k0i1FTTMKw692BknHn5dd1uiPz4JX44oVFbBIfbYKuU1/OJYmLwXf54pH78iPrzZegZz+sLX9sIXXzDF/AEa3G9FmCg/EzKb7SGymdCEvrCTrfjrrTPkwdfLNTxEdgqBo2N3h7mir5XNhgQNH4H5+BVASOMdeJQ98Kx2O5eIOWULS8sr9z7Rk4pMiMFRjRPqoKd80+tgg9OqNU4/+DkvYLFp4NCmOHC1a8an5bA4Fi7t8MnDyuOvxnw2V2ARw7ylK753QG3M1jrPhul8JbqXDgLP4k0LS/l5Pwcw6wRW/dj1sAfIHWcOie6kWIts3po8H4uwXsM8EIlQ/H5lwCLNcQJJsXZYfCa63a5hPfTjXgMrXTdgt8FpT9JDUMeHith7WBliccGeoLX7BXQUc9gkzziZCgFcigsEn3q4AKTehp9Cx9vy45QuHQ++iioMq0on4yauGvs8mPFJIJvlJSlyrwzTIOetg+VByk67F23mU1Lz3VmID7gibgsNZ10ZX9palY8r3vPBmrGqxu2q4z0m6Wdt7FWlVoR+WA01n+ahX0UxPsQWD6UnvY+xlGK3cJQfm5Wr5wXjx+35QbAt5m3B8qHdU55fqHlpimuGnJGqyvgiHvv3fLh0UvFjFPyBhKavsdwqeVZ1jg8lfx27YFw3i7V2OsX5/PnJuPETx2ILiT+pmQja3/juA/VVOb/3BzX/A/7q67uN4fpt7X1vlv8i7/j6XmGsCeqPUyk+4Nd8Kb6F93wpY9ND+ZILqoRJBaXvG7t3fIqXUCVMKij9yNi9I1RcQpUwqaBKmFRQ+rGxe8eoOEOVMKmgnxF27yAVJ+hnhN07SMUJSj9h7N5BKk7Qzwi7d5CKE8qXXNhKmFTYnxJ27ygVR+xLYUrS5LFtYYx47p/o0+d4Gtq9A7kN50Zfnj83ZGReDN9oZLmc8QdXfxdV+NJi84MLHVfXg18iFTcDaql170Buw82u/Yqf8EUCpp1l0VeaNHLlPee/SN/wR0/a+8j9a2+OHn2VH04SfyTcL8PE/S+ece84biX0r9zh5Mv+wNc0hf1zvpxXvjTtUhiZurB/zxcXpnFfQphdhPrZV+FTMm1hl76cHKnCaIpx/o0bfDlHX1yYPeu8UwOjqWlPvEu89OUmnWm2XWNO6f66D7jFl3P0hcLstEVfQozwRYetMfH0hL30FRJqu2EzqRtY3+cmX84rX1pf5AUj6GvGispyiGaVdVHFU7v3mrz2NZx8ntR4XlYVikUZtcIJd5FX+9IvfdnCF7GCzOyCmNA0y9q2SflGhxv59IS95atMLKK3gSkC1tPGNJt8Sj8pdMn1vvQ/fLkZrrodM6i1tCk0rK4e3yAUN34k5q/wli/+N+S/81UkMSka/utjTXzHGN/ji75s9OVGeIqUMDzHNOO/T5QwLW1xDLeS/kdi/gpv+fJwHAvED3EEJsk6t67rzrxbhO9zgy/96EvM59FX3JQajmGZT9LW1gZfMyFODl8Me4VEXOeZtXaQdUgw1Tunb/GlOzSI0FcZ68KXNfgKCsLn84OvVCJffhJpwxyxbbXAZGVZMvbXHO7Lzb6weYVNT5zOdMoG58XY51tv+JraROsNX2WWEa01MWC7mZG2o/w3Pa4tlt/iJl/64Mtq0jJMKo2ajeVEQetqkvlqZlYch1kgZhi5U6dNRKwmd738/zTfOPqy9SpJkplDaZ0ahmF6hM7E+DVn2oxXV2vOpu3LaPAEglz87GXRGAbqIlrMN4qpxX3kdl/8OmJd1sOsw8MNHMNsh1+V0imx+XUp6tDJXZK69KU5w4evwzt23zvjBrv+Y/ff4mu+xBXEi8v0FxcOj1frfyTq2/nnrs+7J1/OuAKT6lMw5evv329Tvr6f6325wlepfN2Fq7+/IXzZuD45faQsFYW47uR0sv401eyN/xLzLsKXwzKzNWVkFBXLGT3Gf63g4Wu8Do0vwFWnJQenZbB770huo7xWFzl+7fo8bknYK/5DnL4mL74Y8PGE497x/usoX3KhfMnF6b4h5UsKlC+5UL7kQvmSC+VLLpQvuVC+5EL5kgvlSy6UL7lQvuRC+ZIL5UsulC+5UL7kQvmSC+VLLpQvuVC+5EL5kgvlSy6UL7lQvuRC+ZIL5UsulC+5UL7kQvmSC+VLLpQvuVC+5EL5kor/AILK+Cj8jWv3AAAAAElFTkSuQmCC align="center")

### 2\. Number

The `<input type="number">` is used to take numbers as input from the user. We can also use the "min" and "max" attributes to specify the minimum number and maximum number. The "value" attribute is used to define a default value.

![](https://i0.wp.com/css-tricks.com/wp-content/uploads/2015/03/numeric-input-opera.gif?ssl=1 align="center")

### 3\. Checkbox

The `<input type="checkbox">` is used to take one or more values as input from the user. We have to use the "value" attribute to specify the value of the checkbox. Here we can also be marked as default by using "checked" inside the input element.

![](https://cdn.educba.com/academy/wp-content/uploads/2020/02/HTML-checkbox-Tag-1.jpg align="center")

### 4\. Radio

The `<input type="radio">` is used to one input from multiple inputs. We have to specify the values by using the value attribute. We can also be marked by default by using "checked" inside the input element.

![](https://static.javatpoint.com/javascriptpages/images/how-to-check-a-radio-button-using-javascript2.png align="center")

### 5\. Color

The `<input type="color">` is used to specify the color as input. Here we can also specify the default color by using the value attribute.

![](https://global.discourse-cdn.com/business7/uploads/plot/optimized/2X/3/30cbdb10cef88fcbc488cd5f5cdc6dd6df93c54d_2_690x289.png align="center")

### 6\. Email

The `<input type="email">` is used to take email as input. The input is not in email format it will show a pop-up. It takes only the email as input if user enter any other input it will show a pop-up to correct it.

![](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/email/email-pattern-match-bad.png align="center")

### 7\. Range

The `<input type="range">` is used to take number input where the exact value is not important. By default value is 1 to 100 but we can specify the min and max attributes.

![](https://assets.hongkiat.com/uploads/html5-form-input-type/range-value.jpg align="center")

### 8\. Date

The `<input type="date">` is used to take a date as input from the user. Here we can also specify the min date and max date.

![](https://i.stack.imgur.com/hblFS.png align="center")

### 9\. Time

The `<input type="time">` is used to take time from the user.

![](https://linuxhint.com/wp-content/uploads/2022/02/input-types-html-16.png align="center")

### 10\. Datetime-local

The `<input type="datetime-local">` is used to take the date and time together.

![](https://i.ytimg.com/vi/GId9jKo5VyM/maxresdefault.jpg align="center")

### 11\. Tel

The `<input type="tel">` is used to take the telephone number from the user. We can use the maxlength attribute to specify the length of the telephone number.

![](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/tel/phone-number-with-options.png align="center")

### 12\. Password

The `<input type="password">` is used to take the password from the user. The letters inside the password are hidden.

![](https://www.csestack.org/wp-content/uploads/2021/02/password-show-hide-for-login-form.png align="center")

### 13\. Submit

The `<input type="submit">` is used to submit the form data to the server using the "method" attribute inside the form tag. The method has two values "get" and "post".

![](https://tutorial.eyehunts.com/wp-content/uploads/2021/06/HTML-form-submit-on-Enter-Key.jpg align="center")

### 14\. Button

The `<input type="button" onclick="fun()" value="click">` is used to create a clickable function. The "onclick" attribute is used to declare the javascript function.

![](https://res.cloudinary.com/practicaldev/image/fetch/s--tLsnN_gJ--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/3bjx4srkfx0v7uf8ci0m.PNG align="center")

### 15\. File

The `<input type="file">` is used to take the input as a file. We can take multiple files also by using the "multiple" inside the input tag.

![](https://i.stack.imgur.com/fvHMu.gif align="center")

### 16\. Month

The `<input type="month">` is used to take month and year from the user.

![](https://linuxhint.com/wp-content/uploads/2022/02/input-types-html-20.png align="center")

### 17\. Week

The `<input type="week">` is used to take the week from the user.

![](https://tubemint.com/wp-content/uploads/2020/08/html-5-input-week-data-type.png align="center")

### 18\. Reset

The `<input type="reset">` is used to reset the user-entered data in the form.

![](https://www.w3.org/TR/html401/images/form_exmpl.gif align="center")

soo these are all types of input elements.