<!-- AR.js by @jerome_etienne - github: https://github.com/jeromeetienne/ar.js - info: https://medium.com/arjs/augmented-reality-in-10-lines-of-html-4e193ea9fdbf -->
<script src="https://aframe.io/releases/0.8.0/aframe.min.js"></script>
<script src="https://cdn.rawgit.com/jeromeetienne/AR.js/1.6.0/aframe/build/aframe-ar.js"></script>
<body style='margin : 0px; overflow: hidden;'>
<!-- initialize AR scene -->	
   <a-scene embedded arjs='sourceType: webcam;'>
<!-- define assets -->
<a-assets>
   <imd id="" src="">
</a-assets>
<!-- setup scene for Spitalfields Roman Woman coffin -->	
		<a-marker preset='custom' type='pattern'     url='https://cdn.rawgit.com/JonoMacC/git-galore/master/scallop_shell.patt'>
          <a-text value="Spitalfields Roman Woman" position='0 0.5 0' rotation='0 45 0'></a-text>
         <a-sphere position='0 1 0' material='opacity: 0.5; color: #4CC3D9; radius: 0.5;'></a-sphere>
      </a-marker>
<!-- setup scene for copperplate map windmills -->      
      <a-marker preset='custom' type='pattern' url='https://cdn.rawgit.com/JonoMacC/git-galore/master/windmill.patt'>
         <a-box position='0 0.5 0' material='opacity: 0.5; color: blue;'></a-box>
      </a-marker>
<!-- setup scene for christ church spitalfields -->      
      <a-marker preset='hiro' type='pattern' url='https://cdn.rawgit.com/JonoMacC/git-galore/master/church_spire.patt'>
         <a-box position='0 0.5 0' material='opacity: 0.5; color: green;'></a-box>
      </a-marker>
      <a-entity camera></a-entity>
	</a-scene>
</body>
