

### Class Files

- Categorize classes into folders. `activities`, `fragments`, `adapters`, `models`, `...` (?) 
- For classes that extend an Android component, the name of the class should end with the name of the component. Each word should start with uppercase. `SignInActivity`, `SignInFragment`, `ImageUploaderService`, `ChangePasswordDialog`

### Object Naming 

- Object names start with lowercase, each subsequent words should start with uppercase. `userOne`, `bluetoothDevice`
- Acronyms should only capitalize the first letter. For example, `functionUrl` and `unitId`. Not `unitID`.
- Constants should be all caps with underscores. `PI_NUMBER`

### Method Naming

- Method names start with lowercase, each subsequent words should start with uppercase. `takeNumbers`

### Resources Files

- Resources file names are written in __lowercase_underscore__.

- Resource files in the values folder should be __plural__. `activity_main.xml`,`ic_launcher_background.xml`, `styles.xml`, `colors.xml`, `dimens.xml`, `attrs.xml`

- When an XML element doesn't have any contents, you must use self closing tags. `<TextView ... />`

### Attributes Order 

1. View Id
2. Style
3. Layout width and layout height
4. Other layout attributes, sorted alphabetically
5. Remaining attributes, sorted alphabetically

    Also group similar attributes together.

### ID Naming

- ID names in xml should be written in __lowercase_underscore__.

	| Element            | Prefix            |
	| -----------------  | ----------------- |
	| `TextView`           | `tv_`  	 | 
	| `EditText`           | `et_`           |
	| `ImageView`          | `img_`		|
	| `Button`             | `btn_`  	 |
	| `ToggleButton`       | `tglbtn_`    	 |
	| `Checkbox`           | `chk_`              |
	| `RadioButton`        | `rb_`               |
	| `Spinner`            | `spn_`              |
	| `ListView`           | `lv_`               |
	| `Menu`               | `menu_`             |

- Activity_ActivityName_ViewType_Description. `activity_main_tv_name`, `fragment_score_button_okay`

### Colors.xml

- For color, use names like `gray_light`, not `button_foreground`.


### Strings.xml

- Use names like `error_msg_network`, `error_msg_call` not `network_error`, `call_failed`. 

- Don't write string values in all uppercase. Stick to normal text conventions (e.g., capitalize first character). If you need to display the string in all caps, then do that using for instance the attribute textAllCaps on a TextView.

### Dimens.xml

- For dimens, use names like `spacing_large`, `spacing_huge`, `font_large` not `button_upper_padding`

### Layout files

- Layout files should match the name of the Android components that they are intended for but moving the top level component name to the beginning. 
	For example, if we are creating a layout for the `SignInActivity`, the name of the layout file should be `activity_sign_in.xml`.

	| Component        | Class Name             | Layout Name                   |
	| ---------------- | ---------------------- | ----------------------------- |
	| Activity         | `UserProfileActivity`  | `activity_user_profile.xml`   |
	| Fragment         | `SignUpFragment`       | `fragment_sign_up.xml`        |
	| Dialog           | `ChangePasswordDialog` | `dialog_change_password.xml`  |
	| AdapterView item | ---                    | `item_person.xml`             |
	| Partial layout   | ---                    | `partial_stats_bar.xml`       |

	A slightly different case is when we are creating a layout that is going to be inflated by an `Adapter`, e.g to populate a `ListView`. In this case, the name of the layout should start with `item_`.

	Note that there are cases where these rules will not be possible to apply. For example, when creating layout files that are intended to be part of other layouts. In this case you should use the prefix `partial_`.

### Drawable files

- Naming conventions for drawables:


	| Asset Type   | Prefix            |		Example              |
	|--------------| ------------------|-----------------------------|
	| Action bar   | `ab_`             | `ab_stacked.9.png`          |
	| Button       | `btn_`	           | `btn_send_pressed.9.png`    |
	| Dialog       | `dialog_`         | `dialog_top.9.png`          |
	| Divider      | `divider_`        | `divider_horizontal.9.png`  |
	| Icon         | `ic_`	           | `ic_star.png`               |
	| Menu         | `menu_	`          | `menu_submenu_bg.9.png`     |
	| Notification | `notification_`   | `notification_bg.9.png`     |
	| Tabs         | `tab_`            | `tab_pressed.9.png`         |


- Naming conventions for icons:

	| Asset Type                      | Prefix             | Example                      |
	| --------------------------------| ----------------   | ---------------------------- |
	| Icons                           | `ic_`              | `ic_star.png`                |
	| Launcher icons                  | `ic_launcher`      | `ic_launcher_calendar.png`   |
	| Menu icons and Action Bar icons | `ic_menu`          | `ic_menu_archive.png`        |
	| Status bar icons                | `ic_stat_notify`   | `ic_stat_notify_msg.png`     |
	| Tab icons                       | `ic_tab`           | `ic_tab_recent.png`          |
	| Dialog icons                    | `ic_dialog`        | `ic_dialog_info.png`         |

- Naming conventions for selector states:

	| State	       | Suffix          | Example                     |
	|--------------|-----------------|-----------------------------|
	| Normal       | `_normal`       | `btn_order_normal.9.png`    |
	| Pressed      | `_pressed`      | `btn_order_pressed.9.png`   |
	| Focused      | `_focused`      | `btn_order_focused.9.png`   |
	| Disabled     | `_disabled`     | `btn_order_disabled.9.png`  |
	| Selected     | `_selected`     | `btn_order_selected.9.png`  |


Source:  	
		
    https://github.com/ribot/android-guidelines/blob/master/project_and_code_guidelines.md

    https://github.com/futurice/android-best-practices
		
    https://stackoverflow.com/questions/12870537/android-naming-convention
		
    https://stackoverflow.com/questions/35923922/best-practices-for-id-naming-conventions-in-android
