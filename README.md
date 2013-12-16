---- Minecraft Crash Report ----
// Oh - I know what I did wrong!

Time: 12/15/13 10:13 PM
Description: Ticking tile entity

java.lang.NullPointerException
	at gregtechmod.api.BaseMetaTileEntityMJ.powerRequest(BaseMetaTileEntityMJ.java:51)
	at buildcraft.transport.PipeTransportPower.updateEntity(PipeTransportPower.java:164)
	at buildcraft.transport.Pipe.updateEntity(Pipe.java:166)
	at buildcraft.transport.TileGenericPipe.g(TileGenericPipe.java:189)
	at yc.h(World.java:2153)
	at in.h(WorldServer.java:516)
	at net.minecraft.server.MinecraftServer.r(MinecraftServer.java:680)
	at ho.r(DedicatedServer.java:269)
	at net.minecraft.server.MinecraftServer.q(MinecraftServer.java:599)
	at net.minecraft.server.MinecraftServer.run(MinecraftServer.java:497)
	at fy.run(SourceFile:849)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at gregtechmod.api.BaseMetaTileEntityMJ.powerRequest(BaseMetaTileEntityMJ.java:51)
	at buildcraft.transport.PipeTransportPower.updateEntity(PipeTransportPower.java:164)
	at buildcraft.transport.Pipe.updateEntity(Pipe.java:166)
	at buildcraft.transport.TileGenericPipe.g(TileGenericPipe.java:189)

-- Tile entity being ticked --
Details:
	Name: net.minecraft.src.buildcraft.transport.GenericPipe // buildcraft.transport.TileGenericPipe
	Block type: ID #0
	Block data value: Unknown? (Got -1)
	Block location: World: (754,66,-107), Chunk: (at 2,4,5 in 47,-7; contains blocks 752,0,-112 to 767,255,-97), Region: (1,-1; contains chunks 32,-32 to 63,-1, blocks 512,0,-512 to 1023,255,-1)
Stacktrace:
	at yc.h(World.java:2153)
	at in.h(WorldServer.java:516)

-- Affected level --
Details:
	Level name: 15362173
	All players: 0 total; []
	Chunk stats: ServerChunkCache: 643 Drop: 0
	Level seed: -4279914292971795785
	Level generator: ID 00 - default, ver 1. Features enabled: true
	Level generator options: 
	Level spawn location: World: (-16,64,256), Chunk: (at 0,4,0 in -1,16; contains blocks -16,0,256 to -1,255,271), Region: (-1,0; contains chunks -32,0 to -1,31, blocks -512,0,0 to -1,255,511)
	Level time: 2456126 game time, 2814482 day time
	Level dimension: 0
	Level storage version: 0x04ABD - Anvil
	Level weather: Rain time: 37949 (now: false), thunder time: 4777 (now: false)
	Level game mode: Game mode: survival (ID 0). Hardcore: false. Cheats: false
Stacktrace:
	at net.minecraft.server.MinecraftServer.r(MinecraftServer.java:680)
	at ho.r(DedicatedServer.java:269)
	at net.minecraft.server.MinecraftServer.q(MinecraftServer.java:599)
	at net.minecraft.server.MinecraftServer.run(MinecraftServer.java:497)
	at fy.run(SourceFile:849)

-- System Details --
Details:
	Minecraft Version: 1.4.7
	Operating System: Linux (amd64) version 2.6.32-358.el6.x86_64
	Java Version: 1.7.0_45, Oracle Corporation
	Java VM Version: OpenJDK 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 751607296 bytes (716 MB) / 1035993088 bytes (988 MB) up to 1035993088 bytes (988 MB)
	JVM Flags: 3 total; -Xmx1024M -Xms1024M -XX:PermSize=1024M
	AABB Pool Size: 1303 (72968 bytes; 0 MB) allocated, 1303 (72968 bytes; 0 MB) used
	Suspicious classes: FML and Forge are installed
	IntCache: cache: 0, tcache: 0, allocated: 3, tallocated: 63
	FML: MCP v7.26a FML v4.7.35.556 Minecraft Forge 6.6.2.534 89 mods loaded, 89 mods active
	mcp [Minecraft Coder Pack] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	FML [Forge Mod Loader] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Forge [Minecraft Forge] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	CodeChickenCore [CodeChicken Core] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	NotEnoughItems [Not Enough Items] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	PowerCrystalsCore [PowerCrystals Core] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MiscPeripheralsASM [MiscPeripherals ASM] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	CoFHCore [CoFH Core] (CoFHCore.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Core [BuildCraft] (buildcraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ComputerCraft [ComputerCraft] (computercraft.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	CCTurtle [ComputerCraft Turtles] (computercraft.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ThermalExpansion [Thermal Expansion] (thermalexpansion.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	OmniTools [OmniTools] (omnitools.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	IC2 [IndustrialCraft 2] (IC2.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	TwilightForest [The Twilight Forest] (TwilightForest.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Builders [BC Builders] (buildcraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Energy [BC Energy] (buildcraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Factory [BC Factory] (buildcraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Transport [BC Transport] (buildcraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Silicon [BC Silicon] (buildcraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	factorization [Factorization] (factorization.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ExtrabiomesXL [ExtrabiomesXL] (ExtrabiomesXL-universal-1.4.7-3.11.0.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Forestry [Forestry for Minecraft] (forestry.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Railcraft [Railcraft] (railcraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	RedPowerCore [RedPower] (redpowercore.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	RedPowerBase [RP Base] (redpowercore.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	RedPowerMachine [RP Machine] (redpowermechanical.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	RedPowerCompat [RP Compat] (redpowercompat.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	RedPowerWiring [RP Wiring] (redpowerdigital.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	RedPowerLogic [RP Logic] (redpowerdigital.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	RedPowerLighting [RP Lighting] (redpowerdigital.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	RedPowerWorld [RP World] (redpowermechanical.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	RedPowerControl [RP Control] (redpowermechanical.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ThermalExpansion|Factory [Factory] (thermalexpansion.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ThermalExpansion|Energy [Energy] (thermalexpansion.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ThermalExpansion|Transport [Transport] (thermalexpansion.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ImmibisCore [Immibis Core] (immibis-core-52.4.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Tubestuff [Tubestuff] (tubestuff.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	XyCraft [§3XyCraft] (xycraft.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	GregTech_Addon [GregTech-Addon] (GregTech.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MiscPeripherals [MiscPeripherals] (miscperipherals-3.1c.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	AppliedEnergistics [Applied Energistics] (AppliedEnergistics.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BiblioCraft [BiblioCraft] (BiblioCraft.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ChargePads [Charge Pads] (ChargePads.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ChickenChunks [ChickenChunks] (ChickenChunks 1.3.1.2.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	EnderStorage [EnderStorage] (EnderStorage.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	FlatBedrock [FlatBedrock] (FlatBedrock.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	GraviGun [GraviGun] (GraviGun.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	IC2NuclearControl [Nuclear Control] (IC2NuclearControl.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	IronChest [Iron Chest] (IronChest.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded [Minefactory Reloaded] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatExtraBiomes [MFR Compat: ExtraBiomes] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatForestry [MFR Compat: Forestry] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatIC2 [MFR Compat: IC2] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatPams [MFR Compat: Pam's Mods] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatRP2 [MFR Compat: RP2] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	SoulShards [SoulShards] (soulshards.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatSoulShards [MFR Compat: Soul Shards] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatSufficientBiomes [MFR Compat: Sufficient Biomes] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Thaumcraft [Thaumcraft] (Thaumcraft.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatThaumcraft [MFR Compat: Thaumcraft] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatTwilightForest [MFR Compat: TwilightForest] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatVanilla [MFR Compat: Vanilla] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	XyCraftWorld [§2XyCraft World] (xycraft.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	MFReloaded|CompatXyCraft [MFR Compat: XyCraft] (MineFactoryReloaded.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	mmmPowersuits [MachineMuse's Modular Powersuits] (ModularPowersuits.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	NetherOres [Nether Ores] (NetherOres.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	PortalGun [Portal Gun] (PortalGun.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	PowerConverters [Power Converters] (PowerConverters.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	StevesCarts [Steve's Carts] (StevesCarts.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	XReliquary [Xeno's Reliquary] (XReliquary.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	AdvancedMachines [IC2 Advanced Machines Addon] (advancedmachines.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	AdvancedSolarPanel [Advanced Solar Panels] (advancedsolarpanel.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	EE3 [Equivalent Exchange 3] (ee3.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BinnieCore [Binnie Core] (extrabees-1.5.0.6b.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ExtraBees [Extra Bees] (extrabees-1.5.0.6b.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	factorization.misc [Factorization Miscellaneous Nonsense] (factorization.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	factorization.dimensionalSlice [Factorization Dimensional Slices] (factorization.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	GraviSuite [Gravitation Suite] (gravisuite.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ModularForceFieldSystem [Modular ForceField System V2] (modularforcefieldsystem.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Mystcraft [Mystcraft] (mystcraft.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ObsidiPlates [Obsidian Pressure Plates] (obsidiplates.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	drceph.petrogen [Petroleum Generator] (petrogen.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	SecretRoomsMod [SecretRoomsMod] (secretroomsmod.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ThaumicBees [ThaumicBees] (thaumicbees.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	WR-CBE|Core [WR-CBE Core] (wirelessredstonecore.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	WR-CBE|Addons [WR-CBE Addons] (wirelessredstoneaddons.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	WR-CBE|RedPower [WR-CBE RedPower] (wirelessredstoneredpower.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	XyCraftMachines [§9XyCraft Machines] (xycraft.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: 154 (8624 bytes; 0 MB) allocated, 154 (8624 bytes; 0 MB) used
	Player Count: 0 / 10; []
	Is Modded: Definitely; Server brand changed to 'forge,fml'
	Type: Dedicated Server (map_server.txt)
