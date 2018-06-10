<!-- AR.js by @jerome_etienne - github: https://github.com/jeromeetienne/ar.js - info: https://medium.com/arjs/augmented-reality-in-10-lines-of-html-4e193ea9fdbf -->
<script src="https://aframe.io/releases/0.8.0/aframe.min.js"></script>
<script src="https://cdn.rawgit.com/jeromeetienne/AR.js/1.6.0/aframe/build/aframe-ar.js"></script>
<body style='margin : 0px; overflow: hidden;'>
<!-- initialize AR scene -->	
   <a-scene embedded arjs='sourceType: webcam; debugUIEnabled: false;'>
<!-- define assets -->
<a-assets>
   <img id="excavate" src="https://cdn.rawgit.com/JonoMacC/git-galore/master/excavations-4.jpg">
   <img id="church" src="https://cdn.rawgit.com/JonoMacC/git-galore/master/Christ_Church_exterior%2C_Spitalfields%2C_London%2C_UK_-_Diliff.jpg">
   <img id="copperplate" src="https://cdn.rawgit.com/JonoMacC/git-galore/master/Copperplate_map_Moorfields.jpg">
</a-assets>
<!-- setup scene for Spitalfields Roman Woman coffin -->	
		<a-marker preset='custom' type='pattern'     url='https://cdn.rawgit.com/JonoMacC/git-galore/master/scallop_shell.patt'>
          <a-entity
  geometry="primitive: plane; width: 2; height: 2"
  material="color: #4FD3FF"
  position="0 0 -1"
  text="value: Roman Woman

This model coffin replicates the approximate shape and patterning of the lead coffin uncovered in Spitalfields in 1999. Dating to between 350 and 410 AD, the coffin contained the remains of a young woman. The scallop shells on the coffin were a common motif on lids of lead coffins in Roman Britain. At this time the area of Spitalfields was still a Roman burial ground and the Roman Woman symbolizes the many buried here. DNA analysis of one of her teeth indicates a possible origin for her in the Basque region of Spain, connecting her to the waves of immigration that have defined Spitalfields throughout its history."></a-entity>
      <a-image
   src="#excavate" 
   width="2" 
   height="2"
   material="color: #A7FF82"
   position="-1 0 0"
   rotation="0 -90 0">
      </a-image>
      </a-marker>
<!-- setup scene for copperplate map windmills -->      
      <a-marker preset='custom' type='pattern' url='https://cdn.rawgit.com/JonoMacC/git-galore/master/windmill.patt'>
        <a-entity
  geometry="primitive: plane; width: 2; height: 2"
  material="color: #4FD3FF"
  position="0 0 -1"
  text="value: Copperplate Map

These windmills are extracted from the Moorfields section of the Copperplate Map of London. Located to the west of Spitalfields, these mills represent some of the industry of the time. The Copperplate Map is the earliest true map of London, dating from between 1553 and 1559. At that time Spitalfields is depicted as being relatively undeveloped."></a-entity>
      <a-image
   src="#copperplate" 
   width="2" 
   height="2"
   material="color: #A7FF82"
   position="-1 0 0"
   rotation="0 -90 0">
      </a-image>
      </a-marker>
<!-- setup scene for christ church spitalfields -->      
      <a-marker preset='custom' type='pattern' url='https://cdn.rawgit.com/JonoMacC/git-galore/master/church_spire.patt'>
        <a-entity
  geometry="primitive: plane; width: 2; height: 2"
  material="color: #4FD3FF"
  position="0 0 -1"
  text="value: Christ Church

Nicholas Hawksmoor's Christ Church has been a fixture of Spitalfields since its construction in 1729, with the model representing its facade. At the time of its completion Spitalfields was full of Huguenot immigrants who fled France to practise their Protestant beliefs without persecution."></a-entity>
      <a-image
   src="#church" 
   width="2" 
   height="2"
   material="color: #A7FF82"
   position="-1 0 0"
   rotation="0 -90 0">
      </a-image>
      </a-marker>
      <a-entity camera></a-entity>
	</a-scene>
</body>
