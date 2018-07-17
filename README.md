# RippleBackground
A beautiful ripple animation for your app. You can easily change its color, speed of wave, one ripple or multiple ripples.


# Ripple-Background
A beautiful ripple animation for your app. You can easily change its color, speed of wave, one ripple or multiple ripples.



Step 1

Install with Gradle

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}


	dependencies {
	        implementation 'com.github.UmeshBaldaniya46:RippleBackground:v1.0'
	}


Step 2

RippleBackground

Add RippleBackground` to your layout with content you want, like an ImageView. Configure the view customization elements using styleable attributes.
 

    <com.ripplebackground.RippleBackground
        android:id="@+id/content"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        app:rb_color="@color/rippelColor"
        app:rb_duration="5000"
        app:rb_radius="30dp"
        app:rb_rippleAmount="6"
        app:rb_scale="6"
        app:rb_strokeWidth="1dp"
        app:rb_type="fillRipple">

        <ImageView
            android:layout_width="30dp"
            android:layout_centerInParent="true"
            android:layout_height="30dp"
            android:src="@drawable/ic_school_black_24dp" />

    </com.ripplebackground.RippleBackground>


Start animation:

RippleBackground rippleBackground=(RippleBackground)findViewById(R.id.content);
rippleBackground.startRippleAnimation();

Stop animation:

rippleBackground.stopRippleAnimation();
