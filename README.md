#AKTabBarController

AKTabBarController is an adaptive and customizable tab bar for iOS.


##Features
- Portrait and Landscape mode tab bar.
- Ability to set the height of the tab bar.
- When the height of the tab bar is too small (inferior to 35px), the title is not displayed. 
- Only one image is needed for both selected and unselected states (style is added via CoreGraphics).
- Images are resized when needed and particularly in landscape mode.
- Animated state of the tabs with a nice cross fade animation.

##Usage
### Creation and initialization of the tab bar
	// Create and initialize the height of the tab bar to 50px.
	self.tabBarController = [[AKTabBarController alloc] initWithTabBarHeight:50];
	
	// Adding the view controllers to manage.
	 [self.tabBarController setViewControllers:[NSMutableArray arrayWithObjects:
                                               [[FirstViewController alloc] init],
                                               [[SecondViewController alloc] init],
                                               [[ThirdViewController alloc] init],
                                               [[FourthViewController alloc] init],nil]
     ];

### Setting the title and image
(in each view controller)

	// Setting the image of the tab.
	- (NSString *)tabImageName
	{
		return @"myImage";
	}
	
	// Setting the title of the tab.
	- (NSString *)tabTitle
	{
		return @"Tab";
	}
	

For further details see the Xcode example project.

##Requirements
- iOS 5.x
- ARC
- QuartzCore.framework

##Screenshots

###iPhone portrait
![iPhone portrait](https://github.com/alikaragoz/AKTabBarController/raw/master/Screenshots/iphone-portrait.png)

###iPhone landscape
![iPhone portrait](https://github.com/alikaragoz/AKTabBarController/raw/master/Screenshots/iphone-landscape.png)

###iPad portrait
![iPhone portrait](https://github.com/alikaragoz/AKTabBarController/raw/master/Screenshots/ipad-portrait.png)

###iPad landscape
![iPhone portrait](https://github.com/alikaragoz/AKTabBarController/raw/master/Screenshots/ipad-landscape.png)

##Todo
- Support any side of the device, particularly for the iPad.
- Ability to set the minimum height of the tab bar to display the title.
- Support different styles (dark, light, etc).
- Ability to set any background pattern.

##Credits
- Largely inspired by **Brian Collins**'s [BCTabBarController](https://github.com/briancollins/BCTabBarController) (for views imbrication).
- Icons used in the example project are designed by **Tomas Gajar** (@tomasgajar).

## Contact

Ali Karagoz

- http://github.com/alikaragoz
- http://twitter.com/alikaragoz

## License

AKTabBarController is available under the MIT license. See the LICENSE file for more info.