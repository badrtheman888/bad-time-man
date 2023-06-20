                            <point x="0.6875" y="0.6875" />
                            <point x="0.3125" y="0.6875" />
                        </collision-poly>
                    </frame>
                </animation>
            </animation-folder>
        </object-type>
        <object-type global="1" name="AttackLoader" sid="6354874427432412">
            <plugin id="Arr" />
        </object-type>
        <object-type global="1" name="MenuStack" sid="1417790766954608">
            <plugin id="Arr" />
        </object-type>
        <object-type name="FileChooser" sid="8898820624476746">
            <plugin id="filechooser" />
        </object-type>
        <object-type name="Browser" sid="4029960250195912">
            <plugin id="Browser" />
        </object-type>
        <object-type name="PlayerHitbox" sid="728293317807613">
            <plugin id="Sprite" />
            <animation-folder>
                <animation framecount="1" loop="0" name="Default" pingpong="0" repeatcount="1" repeatto="0" sid="405047860068601" speed="5">
                    <frame duration="1" hotspotX="0.5" hotspotY="0.5" />
                </animation>
            </animation-folder>
        </object-type>
    </object-folder>
    <families>
        <family name="BoneStab" plugin-id="NinePatch" sid="9321183475132962">
            <members>
                <member>BoneStabH</member>
                <member>BoneStabV</member>
            </members>
            <instance-variables>
                <instance-variable name="Direction" sid="9712410343672045" type="number" />
                <instance-variable name="Distance" sid="1340413306933887" type="number" />
                <instance-variable name="DestX" sid="7626491151499593" type="number" />
                <instance-variable name="DestY" sid="4662037835176925" type="number" />
                <instance-variable name="StayTime" sid="4383237448031349" type="number" />
                <instance-variable name="Reverse" sid="510004270528703" type="boolean" />
            </instance-variables>
        </family>
        <family name="Bone" plugin-id="NinePatch" sid="2013892859044994">
            <members>
                <member>BoneH</member>
                <member>BoneV</member>
            </members>
            <instance-variables>
                <instance-variable name="Direction" sid="2353520185577067" type="number" />
                <instance-variable name="Speed" sid="8541710245044527" type="number" />
            </instance-variables>
        </family>
        <family name="RPGText" plugin-id="Spritefont2" sid="8627438680975019">
            <members>
                <member>BattleFont</member>
                <member>DamageFont</member>
                <member>DefaultFont</member>
                <member>SansFont</member>
            </members>
            <instance-variables>
                <instance-variable name="Name" sid="8126938230629388" type="string" />
                <instance-variable name="Voice" sid="7739643538975967" type="string" />
                <instance-variable name="FullText" sid="4090187800761089" type="string" />
                <instance-variable name="EndFunc" sid="8768540262486332" type="string" />
                <instance-variable name="Interactive" sid="2703717793020135" type="boolean" />
                <instance-variable name="CurrentChar" sid="8429195992300595" type="number" />
                <instance-variable name="T" sid="9067313364631326" type="number" />
                <instance-variable name="Timeout" sid="4487571781562274" type="number" />
            </instance-variables>
            <effects>
                <effect-type name="Tint">
                    <effect id="tint" />
                </effect-type>
            </effects>
        </family>
        <family name="UIButtons" plugin-id="Sprite" sid="9802428034038081">
            <members>
                <member>UIAct</member>
                <member>UIFight</member>
                <member>UIItem</member>
                <member>UIMercy</member>
            </members>
            <instance-variables>
                <instance-variable name="ID" sid="3161584809306413" type="number" />
                <instance-variable name="Action" sid="5414051533652294" type="string" />
            </instance-variables>
        </family>
        <family name="Attack9Patch" plugin-id="NinePatch" sid="9590353435551898">
            <members>
                <member>BoneH</member>
                <member>BoneStabH</member>
                <member>BoneStabV</member>
                <member>BoneStabWarn</member>
                <member>BoneV</member>
                <member>Platform1</member>
                <member>Platform2</member>
            </members>
            <instance-variables>
                <instance-variable name="Damage" sid="6677681737098705" type="number" />
                <instance-variable name="Karma" sid="6030229564139285" type="number" />
                <instance-variable name="Color" sid="821640292253391" type="number" />
            </instance-variables>
            <effects>
                <effect-type name="Tint">
                    <effect id="tint" />
                </effect-type>
            </effects>
        </family>
        <family name="AttackSprite" plugin-id="Sprite" sid="6631597198329078">
            <members>
                <member>GasterBlaster</member>
                <member>MenuBoneBottom</member>
                <member>MenuBoneLeft</member>
            </members>
            <instance-variables>
                <instance-variable name="Damage" sid="1009715326578042" type="number" />
                <instance-variable name="Karma" sid="1305040970412396" type="number" />
            </instance-variables>
        </family>
        <family name="AttackTiled" plugin-id="TiledBg" sid="9784977049754561">
            <members>
                <member>GasterBlastHit</member>
            </members>
            <instance-variables>
                <instance-variable name="Damage" sid="5846064141855004" type="number" />
                <instance-variable name="Karma" sid="4419610502870706" type="number" />
            </instance-variables>
        </family>
        <family name="TouchButton" plugin-id="Sprite" sid="902272746554209">
            <members>
                <member>TouchA</member>
                <member>TouchB</member>
            </members>
            <instance-variables>
                <instance-variable name="TouchID" sid="636958093485166" type="number" />
                <instance-variable name="Pressed" sid="875789127674825" type="boolean" />
            </instance-variables>
        </family>
    </families>
    <layout-folder>
        <layout>BattleScreen.xml</layout>
        <layout>System.xml</layout>
        <layout>MainMenu.xml</layout>
    </layout-folder>
    <event-folder>
        <event-sheet>Battle.xml</event-sheet>
        <event-sheet>InputManagement.xml</event-sheet>
        <event-sheet>Globals.xml</event-sheet>
        <event-sheet>Timeline.xml</event-sheet>
        <event-sheet>Fonts.xml</event-sheet>
        <event-sheet>RPGText.xml</event-sheet>
        <event-sheet>Items.xml</event-sheet>
        <event-sheet>AttackLoader.xml</event-sheet>
        <event-sheet>MainMenu.xml</event-sheet>
        <event-sheet>Menus.xml</event-sheet>
    </event-folder>
    <global-instances>
        <global-instance type="Gamepad" uid="8">
            <properties>
                <analog-deadzone>25</analog-deadzone>
            </properties>
        </global-instance>
        <global-instance type="Keyboard" uid="10" />
        <global-instance type="Function" uid="17" />
        <global-instance type="AJAX" uid="30" />
        <global-instance type="Audio" uid="33">
            <properties>
                <timescale-audio>Off</timescale-audio>
                <saveload>All</saveload>
                <play-in-background>No</play-in-background>
                <positioned-audio></positioned-audio>
                <panning-model>HRTF</panning-model>
                <distance-model>Inverse</distance-model>
                <listener-z-height>600</listener-z-height>
                <reference-distance>600</reference-distance>
                <maximum-distance>10000</maximum-distance>
                <roll-off-factor>1</roll-off-factor>
            </properties>
        </global-instance>
        <global-instance type="Browser" uid="54" />
        <global-instance type="Touch" uid="58">
            <properties>
                <use-mouse-input>Yes</use-mouse-input>
            </properties>
        </global-instance>
    </global-instances>
    <sounds-folder>
        <file name="Ding.ogg" />
        <file name="PlayerFight.ogg" />
        <file name="PlayerDamaged.ogg" />
        <file name="SansSpeak.ogg" />
        <file name="GasterBlaster.ogg" />
        <file name="BoneStab.ogg" />
        <file name="Warning.ogg" />
        <file name="HeartShatter.ogg" />
        <file name="GasterBlast.ogg" />
        <file name="Flash.ogg" />
        <file name="Slam.ogg" />
        <file name="MenuSelect.ogg" />
        <file name="HeartSplit.ogg" />
        <file name="MenuCursor.ogg" />
        <file name="BattleText.ogg" />
        <file name="PlayerHeal.ogg" />
        <file name="GasterBlast2.ogg" />
    </sounds-folder>
    <music-folder>
        <file name="mus_zz_megalovania.ogg" />
    </music-folder>
    <files-folder>
        <file-folder name="Icons">
            <file name="icon-16.png" />
            <file name="icon-32.png" />
            <file name="icon-114.png" />
            <file name="icon-128.png" />
            <file name="icon-256.png" />
            <file name="loading-logo.png" />
        </file-folder>
        <file name="sans_intro.csv" />
        <file name="sans_bonegap1.csv" />
        <file name="sans_bonegap2.csv" />
        <file name="sans_bluebone.csv" />
        <file name="sans_platforms1.csv" />
        <file name="sans_platforms2.csv" />
        <file name="sans_platforms3.csv" />
        <file name="sans_platforms4.csv" />
        <file name="sans_platformblaster.csv" />
        <file name="sans_platforms4hard.csv" />
        <file name="sans_boneslideh.csv" />
        <file name="sans_bonegap1fast.csv" />
        <file name="sans_platformblasterfast.csv" />
        <file name="sans_spare.csv" />
        <file name="sans_bonestab1.csv" />
        <file name="sans_bonestab2.csv" />
        <file name="sans_boneslidev.csv" />
        <file name="sans_multi1.csv" />
        <file name="sans_randomblaster1.csv" />
        <file name="sans_multi2.csv" />
        <file name="sans_randomblaster2.csv" />
        <file name="sans_bonestab3.csv" />
        <file name="sans_multi3.csv" />
        <file name="sans_final.csv" />
    </files-folder>
</c2project>
