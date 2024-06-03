<script setup>

</script>


<template>
    <div class="mech">

        <div class="keyboard">
            <div class="row rowK">
                <div class="key key__esc">
                    <i class="mdi mdi-close"></i>
                </div>
      <div class="key key__symbols">
        ! <span></span> 1
      </div>
      <div class="key key__symbols">
        @ <span></span> 2
      </div>
      <div class="key key__symbols">
        # <span></span> 3
      </div>
      <div class="key key__symbols">
          $ <span></span> 4
        </div>
        <div class="key key__symbols">
        % <span></span> 5
    </div>
      <div class="key key__symbols">
          ^ <span></span> 6
      </div>
      <div class="key key__symbols">
          & <span></span> 7
      </div>
      <div class="key key__symbols">
        * <span></span> 8
      </div>
      <div class="key key__symbols">
        ( <span></span> 9
      </div>
      <div class="key key__symbols">
        ) <span></span> 0
      </div>
      <div class="key key__symbols">
        _ <span></span> -
      </div>
      <div class="key key__symbols">
        + <span></span> =
      </div>
      <div class="key key__delete key__icon">
        <i class="mdi mdi-keyboard-backspace"></i>
      </div>
    </div>
        
    <div class="row rowK">
      <div class="key key__oneandhalf">
        <i class="mdi mdi-keyboard-tab"></i>
    </div>
    <div class="key">
        Q
      </div>
      <div class="key">
        W
      </div>
      <div class="key">
          E
        </div>
        <div class="key">
            R
      </div>
      <div class="key">
          T
      </div>
      <div class="key">
        Y
      </div>
      <div class="key">
        U
      </div>
      <div class="key">
          I
      </div>
      <div class="key">
          O
        </div>
      <div class="key">
        P
    </div>
      <div class="key key__symbols">
        { <span></span> [
        </div>
      <div class="key key__symbols">
        } <span></span> ]
      </div>
      <div class="key key__symbols key__oneandhalf">
        | <span></span> \
      </div>
    </div>
        
    <div class="row rowK">
      <div class="key key__caps">
        <i class="mdi mdi-keyboard-caps"></i>
      </div>
      <div class="key">
        A
      </div>
      <div class="key">
        S
      </div>
      <div class="key">
          D
      </div>
      <div class="key">
        F
    </div>
      <div class="key">
        G
      </div>
      <div class="key">
        H
      </div>
      <div class="key">
        J
      </div>
      <div class="key">
        K
      </div>
      <div class="key">
        L
      </div>
      <div class="key key__symbols">
        : <span></span> ;
      </div>
      <div class="key key__symbols">
        " <span></span> '
      </div>
      <div class="key key__enter">
        <i class="mdi mdi-keyboard-return"></i>
      </div>
    </div>
    
    <div class="row rowK">
      <div class="key key__shift-left">
        <i class="mdi mdi-apple-keyboard-shift"></i>
      </div>
      <div class="key">
        Z
      </div>
      <div class="key">
        X
      </div>
      <div class="key">
        C
      </div>
      <div class="key">
        V
      </div>
      <div class="key">
        B
      </div>
      <div class="key">
        N
      </div>
      <div class="key">
        M
      </div>
      <div class="key key__symbols">
          > <span></span> .
      </div>
      <div class="key key__symbols">
        < <span></span> .
      </div>
      <div class="key key__symbols">
        ? <span></span> /
      </div>
      <div class="key">
        <i class="mdi mdi-apple-keyboard-shift"></i>
      </div>
      <div class="key key__arrow">
        <i class="mdi mdi-chevron-up"></i>
      </div>
      <div class="key">
        <i class="mdi mdi-microphone"></i>
      </div>
    </div>
        
    <div class="row rowK">
      <div class="key key__bottom-funct">
        alt
      </div>
      <div class="key key__bottom-funct">
        func
      </div>
      <div class="key key__bottom-funct">
        cntrl
      </div>
      <div class="key key__spacebar">
      </div>
      <div class="key">
        cntrl
      </div>
      <div class="key">
        alt
      </div>
      <div class="key key__arrow">
        <i class="mdi mdi-chevron-left"></i>
      </div>
      <div class="key key__arrow">
        <i class="mdi mdi-chevron-down"></i>
      </div>
      <div class="key key__arrow">
        <i class="mdi mdi-chevron-right"></i>
    </div>
    </div>
</div>
</div>
</template>


<style lang="scss" scoped>
:root {
  --green: #A2CCB6;
  --yellow: #FCEEB5;
  --peach: #EE786E;
  --off-white: #FFFFF4;
}

span {
  display: block;
  margin-top: -.6%;
}

.mech{
    background-color: #FFFFFF;
  margin-top: 6.4%;
  font-family: Arial;
  font-size: 3px;
  font-style: bold;
}

.keyboard {
    width: 100%;
  height: 100%;
//   width: 780px;
//   height: 262px;
  margin: 0px auto;
  border: .3% solid #000000;
  border-radius: 1%;
  background: #000000;
}

.rowK {
  margin-top: .6%;
  overflow: hidden;
  height: 19%;
}

.key {
  width: 6%;
  float: left;
  cursor: pointer;
  background-color: #FFFFF4;
  color: #000000;
//   line-height: 48px;
  text-align: center;
  margin-left: .6%;
  border-radius: 1%;
}

.key__symbols {
//   line-height: 28px;
}

.key__delete {
  width: 12.8%;
}

.key__oneandhalf {
  width: 9.6%;
}

.key__esc {
  background: #EE786E;
}

.key__enter {
  width: 14.3%;
}

.key__caps {
  width: 11.5%;
}

.key__shift-left {
  width: 12.8%;
}

.key__spacebar {
  width: 37%;
}

.key__bottom-funct {
  width: 8.9%;
}

.key__arrow {
  background-color: #A2CCB6;
}

.mdi {
  margin-top: 1.2%;
}
</style>