<script>
	import SofwareCard from '../components/SoftwareCard.svelte'
</script>

<svelte:head>
	<title>datanist</title>
</svelte:head>

<div class="page test">
	<h1>Software I like</h1>
    <p>On this page you can find a list of software, frameworks etc that I enjoy using.</p>
    <SofwareCard
        title="Godot Game Engine"
        url="https://godotengine.org/"
        desc="Godot is a 2D and 3D, cross-platform, free and open-source game
						engine released under the MIT license. Godot aims to offer a fully
						integrated game development environment. It allows developers to
						create a game from scratch, needing no other tools beyond those used
						for content creation (art assets, music, etc). Games using Godot can
						be created with a variety of programming languages including C++,
						C#, and any other language with GDNative bindings such as Rust, Nim,
						and D."
        imgUrl="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/Godot_icon.svg/1024px-Godot_icon.svg.png"
    />
</div>
