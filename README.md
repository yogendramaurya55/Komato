# Komato---A-food-delivery-app

# Project Structure

  -> Packages

    -> common : we will handle the the database interaction on the basis of response status(constants, utilities, error handlers)
    -> model : we will fetch data from different sources(API calls, Room database, sql lite, etc)
            -> dataModule : sets up how to connect to APIs, databases, etc
            -> repoImplementation : actual workers that fetch/save data (e.g., UserRepositoryImpl gets users from API)
    -> viewModel : Gets data from repository, prepares it, and gives it to UI
            -> repository : contracts (rules) for data fetching (e.g., UserRepository).
            -> viewModule : DI setup for ViewModels
    -> view : UI
             -> components : small reusable widgets (like buttons, cards, text fields).
             -> navigation : tells the app how to move between screens.
             -> screens : full pages of the app (e.g., Login screen, Home screen).

