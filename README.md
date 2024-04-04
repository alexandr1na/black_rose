Feature: Plasarea unei comenzi pe OLX.ro
  As a user
  I want to be able to place an order on OLX.ro
  So that I can purchase items from the platform

  Scenario: Plasarea unei comenzi cu succes
    Given I am on the OLX.ro homepage
    When I search for "laptop" in the search bar
    And I select the first laptop listing from the search results
    And I click on the "Contact" button
    And I fill in the contact form with valid information
    And I click on the "Send" button
    Then I should see a confirmation message indicating that the order was successfully placed
