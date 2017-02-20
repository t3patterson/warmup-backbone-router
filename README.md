# Backbone Router Warmup
### Setup
1. Inside `~/TIY/warmups`, clone this repository 

2. Install the project's packages `npm install`

3. In one terminal tab: 
  - `npm run go` to compile es6 --> es5
  - `npm start` for the webserver

### Task
Use Backbone Router to create routes for:

- `state/:st` : legislators by state
- `gender/:gendr`  :legislators by gender
- `party/:prty/gender/:gen` : legislators by party + gender
- `congressperson/:id` : legislators by id
- `''` (root path) All congress persons


In order to format the `$.getJSON` request properly, will need to reference how to **filter by fields**  on the sunlight foundation api:
https://sunlightlabs.github.io/congress/legislators.html

The request url for retrieving legislator info from the api is:
```
https://congress.api.sunlightfoundation.com/legislators?callack=?
```

It should fetch and render the following UI for each congress person:
```
<div class="profile-card">
	<img src="https://flathash.com/«bioguide_id»">
	<h5>
		«first name»</br>
		<small>«state»</small>
	</h5>
</div>
```