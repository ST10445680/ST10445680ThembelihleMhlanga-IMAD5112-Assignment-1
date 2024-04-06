# ST10445680ThembelihleMhlanga-IMAD5112-Assignment-1
Comprehensive Report: My History App

<u>Introduction:</u>

The My History App is an educational Android application designed to
provide users with insights into historical figures who passed away at
specific ages. This report aims to elucidate the purpose of the app, its
design considerations, and the utilization of GitHub and GitHub Actions
in its development. Additionally, we will delve into a detailed
explanation of the code structure, focusing on the utilization of if and
when statements and the rationale behind the chosen approach.

<u>Purpose of the App:</u>

The primary objective of the My History App is to foster historical
learning in an engaging and accessible manner. By allowing users to
input an age within the range of 20 to 100, the app dynamically
retrieves and displays information about notable individuals who died at
that particular age. This approach aims to personalize historical
learning, making it more relatable and relevant to users. Moreover, the
app seeks to ignite curiosity and interest in history among users of all
ages, serving as a gateway to exploring the past in an interactive and
enjoyable way.

Design Considerations:

<u>User Interface (UI):</u>

The user interface of the My History App is designed with simplicity and
intuitiveness in mind to ensure a seamless user experience. Interactive
elements such as EditText fields for age input and buttons for
generating information and clearing input are strategically placed for
easy access. Visual elements are carefully designed to be visually
appealing while maintaining clarity and readability.

<u>Input Validation:</u>

To enhance the reliability and accuracy of user inputs, robust input
validation mechanisms are implemented in the My History App. When users
input an age, the app verifies that it falls within the specified range
of 20 to 100. If the input age is outside this range or if it is not a
valid numerical value, the app displays clear error messages to guide
users and prompt them to enter valid input.

<u>Display of Information:</u>

The My History App dynamically generates content relevant to the input
age, providing users with insights into notable historical figures who
lived and died during that specific period. Each displayed biography
offers valuable historical context and highlights significant
achievements or contributions of the featured individual. By presenting
information in a concise and engaging manner, the app aims to facilitate
learning and spark curiosity about different historical periods and
figures.

<u>Clear Functionality:</u>

User convenience is prioritized in the design of the My History App,
particularly concerning input management. The inclusion of a "Clear"
button allows users to easily reset the input field, facilitating
subsequent inputs and enhancing the overall user experience. Clear
functionality is designed to be intuitive and easily accessible,
contributing to a seamless and user-friendly interface.

<u>Utilization of GitHub and GitHub Actions:</u>

GitHub serves as a pivotal platform for version control and
collaborative development in the creation of the My History App. It
offers a range of tools and features for managing code repositories,
tracking changes, and facilitating collaboration among developers.
GitHub Actions, a CI/CD tool provided by GitHub, is leveraged for
implementing continuous integration (CI) in the app's development
workflow.

<u>Version Control:</u>

One of the primary functions of GitHub in the development of the My
History App is version control. GitHub enables developers to maintain a
centralized repository of the app's source code, allowing for efficient
tracking of changes, collaboration among team members, and the ability
to revert to previous versions if necessary. By using Git, a distributed
version control system, developers can synchronize their local codebase
with the remote repository hosted on GitHub, ensuring consistency and
collaboration across the development team.

<u>Collaboration:</u>

GitHub facilitates collaboration among developers by providing features
such as pull requests, code reviews, and issue tracking. Pull requests
allow developers to propose changes to the codebase, which can then be
reviewed by other team members before being merged into the main branch.
Code reviews enable peer feedback and ensure code quality, while issue
tracking helps to identify and address bugs, feature requests, and other
issues throughout the development process. These collaborative features
promote transparency, accountability, and efficiency in the development
workflow, enabling the team to work together effectively towards
achieving project goals.

<u>Continuous Integration with GitHub Actions:</u>

GitHub Actions is utilized in the My History App project for
implementing continuous integration (CI), a software development
practice that involves automating the process of integrating code
changes into the main codebase. With GitHub Actions, developers can
define workflows that automate build, test, and deployment processes,
enabling faster feedback loops and more reliable code delivery. CI
pipelines configured with GitHub Actions automatically trigger whenever
changes are pushed to the GitHub repository, ensuring that code changes
are tested and validated before being merged into the main branch. This
helps to catch bugs and issues early in the development cycle, reducing
the risk of introducing defects into the production environment and
improving overall code quality and stability.

Code Explanation:

The code for the My History App is structured in a clear and organized
manner, prioritizing readability, maintainability, and scalability.
Let's delve into a detailed explanation of the code structure and logic:

*<u>User Interface Initialization:</u>*

\- In the \`onCreate\` method, the layout defined in
\`activity\_main.xml\` is inflated and set as the content view of the
activity.
- UI components such as TextViews, EditText fields, and Buttons are
  initialized using their respective IDs obtained from the layout XML
  file.

*<u>Event Listeners Setup:</u>*

- An event listener is attached to the "Generate" button
  (\`btnGenerate\`) using the \`setOnClickListener\` method.

\- When the "Generate" button is clicked, the text entered by the user
in the age input field (\`ageInput\`) is retrieved and stored as a
string (\`userInput\`).

\- The \`toIntOrNull()\` method is used to convert the user input string
to an integer (\`number\`). If the conversion fails (e.g., if the input
is not a valid number), \`null\` is assigned to \`number\`.

*<u>Input Validation:</u>*

- An if statement is used to validate the user input. It checks whether
  \`number\` is not null (indicating successful conversion) and whether it
  falls within the specified age range of 20 to 100.

\- If the user input is valid, the code inside the \`if\` block is
executed; otherwise, the code inside the \`else\` block (not shown here)
handles invalid input.

*<u>Displaying Information Based on User Input:</u>*

- A \`when\` statement is used to handle different scenarios based on
  the user's input age (\`number\`).

\- Each case within the \`when\` block corresponds to a specific age,
and the associated historical information is displayed accordingly.

\- For example, if the user inputs the age 30, the app displays
information about Sylvia Plath, an American poet who died at that age.

*<u>Clearing Input Field:</u>*

- An event listener is attached to the "Clear" button (\`btnClear\`) to
  handle user clicks.

\- When the "Clear" button is clicked, the text input field
(\`ageInput\`) is cleared using the \`clear()\` method.

<img src="/media/image.png" style="width:5in;height:3.125in" />

<img src="/media/image2.png" style="width:5in;height:2.45833in" />

<img src="/media/image3.png" style="width:5in;height:2.38542in" />

<u>Purpose of if and when Statements:</u>

\- \*\*if Statement:\*\* The if statement is used for input validation
to ensure that only valid ages within the specified range (20 to 100)
are accepted. If the user input falls outside this range or is not a
valid numerical value, an error message is displayed to prompt the user
to enter valid input.

When Statement: The when statement is utilized for dynamically
displaying information about historical figures based on the input age.
Each case in the when statement corresponds to a specific age, and the
associated historical information is displayed accordingly. This
approach allows for concise and efficient handling of multiple input
scenarios, making the code more readable and maintainable.

<u>Conclusion:</u>

In conclusion, the My History App serves as an engaging platform for
historical learning, leveraging intuitive design, robust input
validation, and efficient code structure. By providing personalized
insights into historical figures based on user input, the app aims to
make history more accessible and relatable to users of all ages.
Moreover, the utilization of GitHub and GitHub Actions in the app's
development workflow facilitates collaborative development and ensures
code quality and reliability. With continuous development and
enhancements, the My History App endeavors to remain a valuable resource
for historical exploration and knowledge dissemination in the digital
age.

Reference list

II, T. (2017). *25 Legendary Historical Figures Who Died Before Their
Time*. \[online\] List25. Available at:
<https://list25.com/25-legendary-historical-figures-who-died-before-their-time>
\[Accessed 27 Mar. 2024\].

IIE (2024). *Introduction to mobile application development
IMAD5112/d/p/w module manual*.

Jayden (2020). *How History’s Most Famous Figures Died | Daily
Infographic*. \[online\] Daily Infographic | Learn Something New Every
Day. Available at:
<https://www.dailyinfographic.com/famous-figure-deaths> \[Accessed 27
Mar. 2024\].

OpenAI (2022). *ChatGPT*. \[online\] chat.openai.com. Available at:
<https://chat.openai.com> \[Accessed 5 Apr. 2024\].
