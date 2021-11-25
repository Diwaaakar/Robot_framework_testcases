# Robot_framework_testcases

*** Settings ***
Library SeleniumLibrary
Suite Setup     Open browser    ${URL}  ${BROWSER}
Suite Teardown   Close All Browsers

*** Variables ***
${URL}          https://api.mathjs.org/
${BROWSER}      Chrome


*** Test Cases ***
    Open Browsers To Have The Page
    Go to At The End Of The Page
    CLick The Evaluate Button
    An Alert Should Be Open
    Click Ok
    [Teardown]  Close Browser
