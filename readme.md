# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),

# [1.0.3] - In Progress

## 19.01.2023

- Fixed: Issue #64 People search - Similar face search from Actions will show Error dialog
- Fixed: Issue #68 When multiple servers are used, deleting people watchlist failed in specific procedure
- Fixed: Issue #72 Not local time but UTC time is shown for Validity period in face or people registration window
- Fixed: Issue #73 Improve message when the detected face size is under 75 pixel
- Fixed: Issue #74 Some minor improvements in exported HTML file, filter condition
- Fixed: Issue #79 Exception error when uploading gif image for face filter

## 17.01.2023

- Added: Date filters reset on Clear filters
- Fixed: Issue #59 In the Tooltip for Saved filter, Date&time is not shown and bags color text is no need.
- Fixed: Issue #60 "Filter condition", time and camera name in Exported html file is not correct.
- Fixed: Issue #62 [Multiple server registration] Default server name and IP address
- Fixed: Issue #66 Set an upper limit of 31 days for the search date and time period
- Fixed: Issue #67 When ”Search only within : Past month" is used, not 30 days but 31 days is better to be used in API
- Fixed: Issue #69 Exception error when clicking expand filter area button after closing it
- Fixed: Issue #71 Face search result becomes zero due to incorrect coordinate information

## 13.01.2023

- Fixed: Installer not starting Event Server if it was stopped fixed
- Fixed: Issue #54 Fixed Save button not showing up in face registration window
- Fixed: Issue #55 Fixed applying saved filter: dates from utc, selected cameras
- Fixed: Issue #56 Fixed checking cameras by feature
- Fixed: Issue #57 People registering from Actions fixes
- Fixed: Issue #58 Fixed typo
- Fixed: Issue #59 Changes to the tooltip for saved filters
- Fixed: Issue #60 Fixed Html export
- Fixed: Issue #61 Removed TODO message
- Fixed: Issue #65 Fixed search_tumbnail_1 typo

# [1.0.2] - 10.01.2023

- Added: Face Upload
- Added: HTML Export
- Added: Categories for Face Registrations
- Added: Face registration Active Guard Sevrer is automatically set when registering a new tumbnail or changing an existing thumbnail
- Added: Face upload when adding or updating a face registration (saving does not work yet)
- Added: Face upload: with multiple selection for faces
- Added: Face upload: zoom, clear selected photo
- Added: Face upload: padding added to the faces that are close to the margin
- Added: AG Server dropdown list on SetupWatchlists and at Face Watchlist search filters
- Added: MD 3. Export / Snapshot / Move to Playback (TODO: Add camera to playback tab)
- Changed: Camera/Server/FeatureSelection checkboxes selection/deselection
- Changed: MD 2. Filter Selection Square (make check of checkbox bigger)
- Changed: MD 5. Refine Filter (Make Clear All button smaller and make Search button bigger but left it as a tick instead of a square)
- Changed: MD 7. Clear, clears all open results
- Changed: MD 10. Information window, make close a little more obvious
- Changed: MD 12. Larger text on Date/Time (Start-End)
- Changed: MD 14. Better minimising of search filter window on left 
- Fixed: Unable to scroll-down filters on small monitors
- Fixed: Updating an existing face registration doesnt override the representative face
- Fixed: Person registration window
- Fixed: Panel re-sizing
- Fixed: Edit people watchlists UI
- Fixed: Issue #32 Attribute shown in people registration from Actions is not correct
- Fixed: Issue #34 Registered parameter for face watchlist need to be shown for update face registration window
- Fixed: Issue #36 "Cameras" in People watchlist does not work for new registration and update
- Fixed: Issue #37 Detected Info and video playback window can get stuck.
- Fixed: Issue #38 Bottom type detected info in people search is not correct
- Fixed: Issue #41 Add face image to existing face watchlist (Currently only 1 face image can be registered)
- Fixed: Issue #48 "Category" in face watchlist cannot be registered
- Fixed: Issue #49 Exception error occurs if user enter a watchlist name for People watchlist when there is no watchlist registered
- Fixed: Issue #50 Validity period for People watchlist may be unintentionally specified in API
- Fixed: Issue #51 Milestone 2022 - R3 - Active Guard Plugin 1.01 - Face tab
- Fixed: Issue #52 Filter color for bag color and shoes color with Exclude selected color option is not correct
- Fixed: Issue #53 "middle" is used in API when threshold "High" is selected for People search filter

# [1.0.1] - 11.10.2022

- Added: MD 8. Initial Search Message
- Added: MD 11. Lost Thumbnail in Playback Window
- Added: Search by attribute
- Added: Bag, Bag Color, Shoes filter
- Added: Similar face search function
- Added: Search only within: Past 24 hours/Past week/Past month
- Added: Issue #44 Could you support "Clear" face image for face filter ?
- Fixed: Issue #32 Attribute shown in people registration from Actions is not correct
- Fixed: Issue #34 Registered parameter for face watchlist need to be shown for update face registration window
- Fixed: Issue #36 "Cameras" in People watchlist does not work for new registration and update
- Fixed: Issue #38 Bottom type detected info in people search is not correct
- Fixed: Issue #41 Add face image to existing face watchlist (Currently only 1 face image can be registered)
- Fixed: Issue #43 Some filter option for Bag, Bag color and Shoes color should be shown when "Advanced filter" is clicked.
- Fixed: Issue #45 Search result of people search with default filter (just "on") will be always 0
- Fixed: Issue #46 Face image from watchlist cannot be set for face filter
- Fixed: Issue #47 Start and End time for search API is not correct when unchecked for "Search only within" 

# [1.0.0] - 01.07.2022

- Fixed: Setup Watchlist Panel cannot be opened when there are no machtlists in the Active Guard Server
- Fixed: "Include selected camera" filter
- Fixed: Multi-sensor cameras not displayed correctly in playback and camera filter
- Fixed: Cameras not being displayed when the server response contains a GUID as camera ID
- Fixed: The filter page was changing size after minimizing
- Fixed: People registration not displaying the same attributes as the Detected Info panel
- Fixed: Saved Watchlist Panel displaying 0 cameras when cameras are saved
- Fixed: Update Face Registration Panel now automatically fills in with the currently registered attributes
- Fixed: Face Watchlist not searching correctly when "Arbitrary" is selected for gender
- Fixed: Detected Info Panel displaying inverted information between short and long bottom types
- Fixed: Detected Info Panel vehicle info
- Fixed: Vehicle similar search
- Fixed: Save snapshot path containing special characters
- Changed: Action buttons now only display for images that contain their specific registration face/people/vehicle
- Changed: Panels now close when the user clicks outside of them
- Changed: Show/Hide cameras based on AI Capability

# [0.9.7] - 13.05.2022

- Fixed: Adding new watchlist from the Smart Client
- Fixed: The image from the People Watchlist Panel now displays correctly
- Fixed: Fields in the People Watchlist Panel were being set to an incorrect default value
- Fixed: Filter tooltip
- Fixed: The search panel should only display available filters according to API response
- Fixed: Adjusted filters strings to be more user-friendly
- Fixed: Saved filters not saving the date and time
- Fixed: GUI sizing and spelling
- Fixed: Tabs cannot be closed
- Fixed: Json serializer
- Fixed: Face Registration image sent to the server was not cropped
- Fixed: Detected Info displaying the wrong data for Hair_Color: Gold
- Fixed: Right-click on playbacl window crashes the Smart Client
- Fixed: People watchlist fields now reset correctly
- Changed: The Clear and Cancel buttons now cancel / clear the search using the API instead of locally
- Changed: The default value of the video playback start time is now set to 5 seconds before the timestamp on the image
- Removed: Loading Thumbnails from disk

# [0.9.4] - 16.04.2022

- Added: Face Registration Panel
- Added: Update Face Registration Panel
- Added: Thumbnail Face Cropping
- Added: Loading Thumbnails from disk
- Added: Thumbnail Context Menu
- Added: Multi Tab search
- Added: Filters
- Added: Save Filters
- Added: Clear Filters
- Added: Filter Tooltips
- Added: People Registration Panel
- Added: Search Matchlist thumbnails
- Added: Setup Watchlist Panel
- Added: Right Click Menu for face matching
- Added: Clear Button in 
- Fixed: Lazy Loading
- Fixed: DateTime Picker
- Fixed: Delete Face Registration
- Fixed: UI style
- Fixed: Selecting cameras
- Fixed: Sort option
- Changed: Improved search and thumbnail retrieval


# [0.9.2] - 21.03.2022

- Added: Vehicle Search Filters
- Added: Sort thumbnails by Hour
- Added: Load More button
- Added: Thumbnail time and camera name overlay
- Added: Advanced filters only enabled if a filter is selected
- Added: Camera preview and thumbnail information can be hidden
- Added: Selected Thumbnail is highlighted
- Added: All minutes values to time selection
- Added: Check date selection for invalid selections
- Added: Lazy Loading (always active)
- Fixed: Cameras not in Milestone are hidden
- Fixed: Fixed JSONs to not send NULL data when search filter is empty
- Fixed: Date/Time selection sends UTC to the server
- Changed: Paging is used to load thumbnails 100 results at a time
- Changed: Fixed styling for thumbnail scale slide
- Changed: Start time is one day before current time and end time is current time
