# Video State Machine

Here is the state machine with all of the states

 ![alt tag](https://user-images.githubusercontent.com/44596360/101228697-ab5a3a00-3651-11eb-948f-f3e1be86fac4.png)
 ### Explanation of states:
      1) LOADING: Is the initial state where we wait for the video to load
            - ready: If the load was successful we move to this set of states
            - failure: If for whatever reason the video failed to load we move to the fail state
      2) The set of ready states:
            - paused: The video playback is paused
            - playing: The video is playing
            - ended: Video has reached the end
 
 ## The image below is the video player with custom controls
 ![alt tag](https://user-images.githubusercontent.com/44596360/101260936-3259f180-36e8-11eb-8ffe-9134feee28ee.png)
 
### XSTATE
          
          XSTATE:
          - Is a state management library It helps describe application state using finite state machines and statecharts.
            A state machine is a mathematical model of computation, it's an abstract state machine with a finite number of 
            states at any give time.
           
          - Using xstate allowed me to vizualize the states my react video player would have. 
          
          - Initially I just had VideoJS imported into my project and was not able to custom make my own controls with 
            videojs alone. I was only able to hide the deafault controls videojs came with and that wasn't my project 
            requirements so I had to continue my research into making my own video player controls in React. 
            
          - What my search led me to was XSTATE and using this 
            library helped create my own custom controls for a react video player.
            
