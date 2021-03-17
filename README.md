# Curtis
Minecraft ModPack Error: java.lang.NullPointerException: Null string not allowed Exit Code: -1

---- Minecraft Crash Report ----

WARNING: coremods are present:
  CorePlugin (ForgeEndertech-1.12.2-4.5.0.0-build.0435.jar)
  ForgelinPlugin (Forgelin-1.8.4.jar)
  MekanismCoremod (Mekanism-1.12.2-9.8.3.390.jar)
  OpenModsCorePlugin (OpenModsLib-1.12.2-0.12.2.jar)
  CTMCorePlugin (CTM-MC1.12.2-1.0.2.31.jar)
  Fermion ASM Service (Fermion-1.0.2+hotfix.jar)
  LoadingPlugin (Bloodmoon-MC1.12.2-1.5.3.jar)
  WolfArmorCore (wolfarmor-1.12.2-3.7.5-universal-signed.jar)
  llibrary (llibrary-core-1.0.11-1.12.2.jar)
  IELoadingPlugin (ImmersiveEngineering-core-0.12-89.jar)
  AstralCore (astralsorcery-1.12.2-1.10.27.jar)
  Inventory Tweaks Coremod (InventoryTweaks-1.63.jar)
  EnderCorePlugin (EnderCore-1.12.2-0.5.76-core.jar)
  PhosphorFMLLoadingPlugin (phosphor-1.12.2-0.2.6+build50.jar)
  CharmLoadingPlugin (Charm-1.12.2-1.3.6.jar)
Contact their authors BEFORE contacting forge

// Daisy, daisy...

Time: 3/17/21 5:10 AM
Description: Initializing game

java.lang.NullPointerException: Null string not allowed
	at java.util.Objects.requireNonNull(Objects.java:228)
	at net.minecraft.nbt.NBTTagString.<init>(NBTTagString.java:19)
	at net.minecraft.nbt.NBTTagCompound.func_74778_a(NBTTagCompound.java:138)
	at net.minecraftforge.fluids.FluidStack.writeToNBT(FluidStack.java:107)
	at net.minecraftforge.fluids.FluidUtil.getFilledBucket(FluidUtil.java:750)
	at furgl.stupidThings.common.fluid.ModFluids$RegistrationHandler.registerItems(ModFluids.java:72)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler_1264_RegistrationHandler_registerItems_Register.invoke(.dynamic)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler.invoke(ASMEventHandler.java:90)
	at net.minecraftforge.fml.common.eventhandler.EventBus$1.invoke(EventBus.java:144)
	at net.minecraftforge.fml.common.eventhandler.EventBus.post(EventBus.java:182)
	at net.minecraftforge.registries.GameData.fireRegistryEvents(GameData.java:850)
	at net.minecraftforge.fml.common.Loader.preinitializeMods(Loader.java:630)
	at net.minecraftforge.fml.client.FMLClientHandler.beginMinecraftLoading(FMLClientHandler.java:252)
	at net.minecraft.client.Minecraft.func_71384_a(Minecraft.java:467)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:378)
	at net.minecraft.client.main.Main.main(SourceFile:123)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Client thread
Stacktrace:
	at java.util.Objects.requireNonNull(Objects.java:228)
	at net.minecraft.nbt.NBTTagString.<init>(NBTTagString.java:19)
	at net.minecraft.nbt.NBTTagCompound.func_74778_a(NBTTagCompound.java:138)
	at net.minecraftforge.fluids.FluidStack.writeToNBT(FluidStack.java:107)
	at net.minecraftforge.fluids.FluidUtil.getFilledBucket(FluidUtil.java:750)
	at furgl.stupidThings.common.fluid.ModFluids$RegistrationHandler.registerItems(ModFluids.java:72)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler_1264_RegistrationHandler_registerItems_Register.invoke(.dynamic)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler.invoke(ASMEventHandler.java:90)
	at net.minecraftforge.fml.common.eventhandler.EventBus$1.invoke(EventBus.java:144)
	at net.minecraftforge.fml.common.eventhandler.EventBus.post(EventBus.java:182)
	at net.minecraftforge.registries.GameData.fireRegistryEvents(GameData.java:850)
	at net.minecraftforge.fml.common.Loader.preinitializeMods(Loader.java:630)
	at net.minecraftforge.fml.client.FMLClientHandler.beginMinecraftLoading(FMLClientHandler.java:252)
	at net.minecraft.client.Minecraft.func_71384_a(Minecraft.java:467)

-- Initialization --
Details:
Stacktrace:
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:378)
	at net.minecraft.client.main.Main.main(SourceFile:123)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)

