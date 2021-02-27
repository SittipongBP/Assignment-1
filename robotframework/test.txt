*** Settings ***
Library  SeleniumLibrary

*** Variables ***
${HOMEPAGE}  http://www.google.com/?hl=th
${BROWSER}  Chrome

*** Test Cases ***
Go To homepage
  Open Browser  ${HOMEPAGE}  ${BROWSER}