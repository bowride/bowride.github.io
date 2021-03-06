<img src="doc/bowride-logo-small.png">

#### Bowride is a website that will allow users to organize carpools with other members of the UH community. Users can sign up to be a driver or rider, and drivers can search for riders that are most convenient to/from campus. These carpools can be reoccurring such as everyday classes or one-time such as for special events. A rating system for both drivers and passengers prevents abuses, plus a special administrator mode that enables the site admin to remove users based upon substantiated complaints.

## RUN APP HERE!
[BowRide APP](http://bowride.meteorapp.com/#/)

## Our Members
Our Github [Organization](https://github.com/bowride) 

* [Derek Sola](https://derekasola.github.io/)

* [Don Maddock](https://don-maddock.github.io/)

* [Jake Hijirida](https://jakehiji.github.io/)

* [Moseli Motsoehli](https://deepsmoseli.github.io/)

## Milestone 1
A link to our [first Milestone project board.](https://github.com/bowride/bowride/projects/1)

## Milestone 2
A link to our [second Milestone project board.](https://github.com/bowride/bowride/projects/2)

## Milestone 3
A link to our [second Milestone project board.](https://github.com/bowride/bowride/projects/3)

## Developer Guide
First, [install Meteor](https://www.meteor.com/install).

Second, go to [https://github.com/bowride/bowride](https://github.com/bowride/bowride), and click the "Use this template" button. Complete the dialog box to create a new repository that you own that is initialized with this template's files.

Third, go to your newly created repository, and click the "Clone or download" button to download your new GitHub repo to your local file system.  Using [GitHub Desktop](https://desktop.github.com/) is a great choice if you use MacOS or Windows.

Fourth, cd into the app/ directory of your local copy of the repo, and install third party libraries with:

```
$ meteor npm install
```

Last, get a Google Maps API key by following the guide at [https://developers.google.com/maps/documentation/javascript/get-api-key](https://developers.google.com/maps/documentation/javascript/get-api-key) and place it in the [GoogleMaps.jsx file](https://github.com/bowride/bowride/blob/master/app/imports/ui/pages/GoogleMaps.jsx) where it says API_KEY_HERE.

```jsx
export default class SimpleMap extends Component{

  render() {
    return (

        <div className='ui center aligned container' style={{height: '80vh', width: '80vw'}}>
        <GoogleMapReact
            bootstrapURLKeys='API_KEY_HERE'
            defaultCenter={{lat: 21.298872, lng: -157.817204}}
            defaultZoom={ 16 }
        >
          <Marker
              lat={21.298872}
              lng={-157.817204}
              text={'Pick-Up Location'}
          />
        </GoogleMapReact>
        </div>
    );
  }

}
```

## Running the system

Once the libraries are installed, you can run the application by invoking the "start" script in the [package.json file](https://github.com/bowride/bowride/blob/master/app/package.json):

```
$ meteor npm run start
```

## Users Guide

#### Current Landing Page
<img src="doc/Final-Landing.png">

This is the landing page, here you will find info about our web app. Use the top login button or sign up for an account.

#### Login To Your Account
<img src="doc/Final-Login.png">

This is the log in screen where you log into your account.

#### Register For An Account
<img src="doc/Final-Register.png">

If you do not have an account already, you can register for an account on the sign up page.

#### Logged in
<img src="doc/Final-Landing-Logedin.png">

This is the home page when you are signed in.

#### Drivers
<img src="doc/Final-ListDrivers.png">

This is were all the drivers currently signed up are displayed. each driver i required to give their destination for easy picking.

#### I Want To Drive
<img src="doc/Final-I_Want_To_Drive.png">

If you want to be a driver that day you can sign up to be a driver on this page.

#### Google Maps
<img src="doc/Final-Maps.png">

This is a map to find pick up locations for your rides. the markers display the general area for pick up locations for each destination as well as how many drivers are available for that destination.

#### Google Maps _OnChildClick()
<img src="doc/Final-Maps_OnClick.png">

When you click the marker, An alert with some basic info about the pick up location will be displayed.

#### Profile
<img src="doc/Final-Profile.png">

Here is your profile.

#### Edit Driver/Profile
<img src="doc/Final-Edit_Profile.png">

If you need to edit your drivers card or profile, you can do so here.

#### Admin Stats
<img src="doc/Final-Admin.png">

Here, the admin can see data on the apps usage.
