Note: Forked from [here](https://github.com/xpenatan/gdx-bullet-gwt), updated by myself to use gradle and be includable in libGDX projects easily.

# gdx-bullet-gwt
Bullet extension for libgdx html5

This extension emulate java bullet extension to use ammo.js instead of c++ jni. If a error pops in its because the class/method is not yet emulated. Any optimization and adding missing implementation is welcome. 

If you going to help try to keep js calls as low as possible because there is a weird error "Maximum call stack size exceeded" that can occur. 

# Dependencies
(maven and gradle links)

# Instructions
1 - GwtBullet.init() needs to be called before return ApplicationListener at getApplicationListener().  
2 - Have to place bullet.gwt.xml file in gdx-bullet project at com.badlogic.gdx.physics.  
3 - Have to include \<inherits name="com.badlogic.gdx.physics.bullet.bullet-gwt"/> in gwt.xml file.  
4 - For gdx-tests-gwt to work you need to remove System.load from BaseBulletTest.java.




