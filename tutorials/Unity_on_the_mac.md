# How to make Unity use your mac GPU

As explained in [official Unity Docs](https://docs.unity3d.com/560/Documentation/Manual/ComputeShaders.html), on the Mac, Unity uses [Metal](https://developer.apple.com/metal/) to access the GPU hardware. In case your GPU card is a bit old, you may have to force Unity to run with Metal [source](https://forum.unity.com/threads/mac-editor-metal.446365/#post-2888367):

    /Applications/Unity/Unity.app/Contents/MacOS/Unity -force-metal


