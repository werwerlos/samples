<!-- TC title -->
<header><h2>Create Account - form field validation</header>

<!-- Preconditions -->
<h3> Preconditions: </h3>
    <li> User is not logged in.
    <li> User is located on the /create-account page.
<br/><br/>

<!--Steps instruction  and their expected results -->
<table>
    <tr>
        <th>No</th>
        <th>Steps</th>
        <th>Expected results</th>
    </tr>
    <tr>
        <td>1</td>
        <td> 
            <li>Leave form fields empty.</li>
            <li>Click on the <i>Agree and Continue</i> CTA</li>    
        </td>
        <td> 
            <li>Form is not submitted.</li>
            <li>There is a focus on the first field of a form.</li>
            <li>Required inputs (Email and Password) are decorated with a red outline.</li>
            <li>There are inline validation messages under each of the decorated fields.</li>            
            <img width="418" alt="Validation of empty fields" src="images/RegistrationEmptyFieldsValidation.png">
        </td>
    </tr> 
    <tr>
        <td>2</td>
        <td>
            <li>Verify inline error message for the empty Email field.</li>   
        </td>
        <td>
            <li>There is a red icon with an exclamation mark on the left side of the message.</li>
            <li>There is a message displayed informing the user to enter the correct data in order to continue. <i>"Please enter a valid email and password before selecting 'Agree and Continue.'
</i></li> 
        </td>
    </tr>
    <tr>
        <td>3</td>
        <td>
            <li>Verify inline message for empty Password field.</li>  
        </td>
        <td> 
            <li>There is a red icon with an exclamation mark on the left side of the message.</li>
            <li>There is a message displayed informing the user of the password requirements.<i>"Password must contain a minimum of 8 characters, with an uppercase letter, a lowercase letter, and a number.
"</i></li>
        </td>
    </tr><tr>
        <td>4</td>
        <td>
            <li>Enter invalid email into the <i>Email</> field.</li>
            <li>Click on the <i>Agree and Continue</i> CTA.</li>
        </td>
        <td> 
            <li>The is an inline error message displayed informing the user about not valid email.</li>
            <li>There is a focus on the Email field.</li>
            <img width="418" alt="Incorrect email and empty password" src="images/RegistrationIncorectEmail.png">
        </td>
    </tr><tr>
        <td>6</td>
        <td>
            <li>Enter correct email into the <i>Email</i> field.</li>
            <li>Enter invalid password into the <i>Password</i> field</li>
            <li>Click on the <i>Agree and Continue</i> CTA</li>   
        </td>
        <td> 
            <li>There is an inline error informing user about password requirements.</li>
            <li>There is a focus on the Password field.</li>
            <li>There are no errors for the Email field displayed.</li>
            <img width="418" alt="Correct Email with invalid Password" src="images/RegistrationCorrectMailWrongPassword.png">
        </td>
    </tr><tr>
        <td>7</td>
        <td>
            <li>Enter already registered email into the <i>Email</i> field.</li>
            <li>Enter valid password into the <i>Password</i> field</li>
            <li>Click on the <i>Agree and Continue</i> CTA</li>    
        </td>
        <td> 
            <li> A Toast notification with a message about the probability of an already registered account is displayed above the form.</li>
            <li>There are no errors displayed for specific fields.</li>
            <li>There is no focus on neither of fields.</li>
            <img width="418" alt="Already registered user error" src="images/RegistrationAlreadyRegisteredError.png">
        </td>
</table>
