Note: Forked from [here](https://github.com/xpenatan/gdx-bullet-gwt), updated by myself to use gradle and be includable in libGDX projects easily.

# gdx-bullet-gwt
Bullet extension for libgdx html5

This extension emulate java bullet extension to use ammo.js instead of c++ jni. If a error pops in its because the class/method is not yet emulated. Any optimization and adding missing implementation is welcome. 

If you going to help try to keep js calls as low as possible because there is a weird error "Maximum call stack size exceeded" that can occur. 

# Dependencies

I'll put up the compiled jar that I having working for myself + sources if necessary.

Otherwise, simply cloning this project and typing ***gradlew install*** will add it to your local gradle repository.

Then, add:

```$xslt
api "gdx-bullet-gwt:gdx-bullet-gwt:unspecified"
api "gdx-bullet-gwt:gdx-bullet-gwt:unspecified:sources"
```

to your html build.gradle dependencies.

# Instructions (in any particular order)
- Add the gdx-bullet-gwt.jar to your project class path (see dependencies)
- Add ***<script src="html/ammo.js"/>*** * to your index.html
- Bullet.initVariables() needs to be called before return ApplicationListener at getApplicationListener().  
- Have to include \<inherits name="com.badlogic.gdx.physics.bullet.bullet-gwt"/> in gwt.xml file. 
  





