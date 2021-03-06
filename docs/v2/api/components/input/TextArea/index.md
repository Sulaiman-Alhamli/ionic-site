---
layout: "v2_fluid/docs_base"
version: "2.0.0-rc.3"
versionHref: "/docs/v2"
path: ""
category: api
id: "textarea"
title: "TextArea"
header_sub_title: "Ionic API Documentation"
doc: "TextArea"
docType: "class"
show_preview_device: true
preview_device_url: "/docs/v2/demos/src/textarea/"
angular_controller: APIDemoCtrl 
---









<h1 class="api-title">
<a class="anchor" name="text-area" href="#text-area"></a>

TextArea
<h3><code>ion-textarea</code></h3>






</h1>

<a class="improve-v2-docs" href="http://github.com/driftyco/ionic/edit/master//src/components/input/input.ts#L251">
Improve this doc
</a>






<p><code>ion-textarea</code> is is used for multi-line text inputs. Ionic still
uses an actual <code>&lt;textarea&gt;</code> HTML element within the component;
however, with Ionic wrapping the native HTML text area element, Ionic
is able to better handle the user experience and interactivity.</p>
<p>Note that <code>&lt;ion-textarea&gt;</code> must load its value from the <code>value</code> or
<code>[(ngModel)]</code> attribute. Unlike the native <code>&lt;textarea&gt;</code> element,
<code>&lt;ion-textarea&gt;</code> does not support loading its value from the
textarea&#39;s inner content.</p>
<p>When requiring only a single-line text input, we recommend using
<code>&lt;ion-input&gt;</code> instead.</p>




<!-- @usage tag -->

<h2><a class="anchor" name="usage" href="#usage"></a>Usage</h2>

<pre><code class="lang-html"> &lt;ion-item&gt;
   &lt;ion-label&gt;Comments&lt;/ion-label&gt;
   &lt;ion-textarea&gt;&lt;/ion-textarea&gt;
 &lt;/ion-item&gt;

 &lt;ion-item&gt;
   &lt;ion-label stacked&gt;Message&lt;/ion-label&gt;
   &lt;ion-textarea [(ngModel)]=&quot;msg&quot;&gt;&lt;/ion-textarea&gt;
 &lt;/ion-item&gt;

 &lt;ion-item&gt;
   &lt;ion-label floating&gt;Description&lt;/ion-label&gt;
   &lt;ion-textarea&gt;&lt;/ion-textarea&gt;
 &lt;/ion-item&gt;

&lt;ion-item&gt;
   &lt;ion-label&gt;Long Description&lt;/ion-label&gt;
   &lt;ion-textarea rows=&quot;6&quot; placeholder=&quot;enter long description here...&quot;&gt;&lt;/ion-textarea&gt;
 &lt;/ion-item&gt;
</code></pre>




<!-- @property tags -->



<!-- instance methods on the class -->
<!-- input methods on the class -->
<h2><a class="anchor" name="input-properties" href="#input-properties"></a>Input Properties</h2>
<table class="table param-table" style="margin:0;">
  <thead>
    <tr>
      <th>Attr</th>
      <th>Type</th>
      <th>Details</th>
    </tr>
  </thead>
  <tbody>
    
    <tr>
      <td>placeholder</td>
      <td><code>string</code></td>
      <td><p> The placeholder for the textarea</p>
</td>
    </tr>
    
    <tr>
      <td>value</td>
      <td><code>string</code></td>
      <td><p> The value of the textarea</p>
</td>
    </tr>
    
    <tr>
      <td>disabled</td>
      <td><code>bool</code></td>
      <td><p> Wheather the textarea should be disabled or not</p>
</td>
    </tr>
    
    <tr>
      <td>mode</td>
      <td><code>string</code></td>
      <td><p> The mode to apply to this component.</p>
</td>
    </tr>
    
  </tbody>
</table>
<!-- output events on the class -->
<h2><a class="anchor" name="output-events" href="#output-events"></a>Output Events</h2>
<table class="table param-table" style="margin:0;">
  <thead>
    <tr>
      <th>Attr</th>
      <th>Details</th>
    </tr>
  </thead>
  <tbody>
    
    <tr>
      <td>blur</td>
      <td><p> Expression to call when the textarea no longer has focus</p>
</td>
    </tr>
    
    <tr>
      <td>focus</td>
      <td><p> Expression to call when the textarea has focus</p>
</td>
    </tr>
    
  </tbody>
</table>


  <h2 id="sass-variable-header"><a class="anchor" name="sass-variables" href="#sass-variables"></a>Sass Variables</h2>
  <div id="sass-variables" ng-controller="SassToggleCtrl">
  <div class="sass-platform-toggle">
    
      
      
      <a ng-init="setSassPlatform('base')" ng-class="{ active: active === 'base' }" ng-click="setSassPlatform('base')" >All</a>
      
      
      
      <a ng-class="{ active: active === 'ios' }" ng-click="setSassPlatform('ios')">iOS</a>
      
      
      
      <a ng-class="{ active: active === 'md' }" ng-click="setSassPlatform('md')">Material Design</a>
      
      
      
      <a ng-class="{ active: active === 'wp' }" ng-click="setSassPlatform('wp')">Windows Platform</a>
      
      
    
  </div>


  
  <table ng-show="active === 'base'" id="sass-base" class="table param-table" style="margin:0;">
    <thead>
      <tr>
        <th>Property</th>
        <th>Default</th>
        <th>Description</th>
      </tr>
    </thead>
    <tbody>
      
      <tr>
        <td><code>$text-input-highlight-color-valid</code></td>
        
          <td><code>#32db64</code></td>
        
        <td><p>Color of the input highlight when valid</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-highlight-color-invalid</code></td>
        
          <td><code>#f53d3d</code></td>
        
        <td><p>Color of the input highlight when invalid</p>
</td>
      </tr>
      
    </tbody>
  </table>
  
  <table ng-show="active === 'ios'" id="sass-ios" class="table param-table" style="margin:0;">
    <thead>
      <tr>
        <th>Property</th>
        <th>Default</th>
        <th>Description</th>
      </tr>
    </thead>
    <tbody>
      
      <tr>
        <td><code>$text-input-ios-background-color</code></td>
        
          <td><code>$list-ios-background-color</code></td>
        
        <td><p>Background color of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-margin-top</code></td>
        
          <td><code>$item-ios-padding-top</code></td>
        
        <td><p>Margin top of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-margin-right</code></td>
        
          <td><code>($item-ios-padding-right / 2)</code></td>
        
        <td><p>Margin right of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-margin-bottom</code></td>
        
          <td><code>$item-ios-padding-bottom</code></td>
        
        <td><p>Margin bottom of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-margin-left</code></td>
        
          <td><code>0</code></td>
        
        <td><p>Margin left of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-input-clear-icon-width</code></td>
        
          <td><code>30px</code></td>
        
        <td><p>Width of the icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-input-clear-icon-color</code></td>
        
          <td><code>rgba(0, 0, 0, .5)</code></td>
        
        <td><p>Color of the icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-input-clear-icon-svg</code></td>
        
          <td><code>&quot;&lt;svg xmlns=&#39;http://www.w3.org/2000/svg&#39; viewBox=&#39;0 0 512 512&#39;&gt;&lt;path fill=&#39;&quot; + $text-input-ios-input-clear-icon-color + &quot;&#39; d=&#39;M403.1,108.9c-81.2-81.2-212.9-81.2-294.2,0s-81.2,212.9,0,294.2c81.2,81.2,212.9,81.2,294.2,0S484.3,190.1,403.1,108.9z M352,340.2L340.2,352l-84.4-84.2l-84,83.8L160,339.8l84-83.8l-84-83.8l11.8-11.8l84,83.8l84.4-84.2l11.8,11.8L267.6,256L352,340.2z&#39;/&gt;&lt;/svg&gt;&quot;</code></td>
        
        <td><p>Icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-input-clear-icon-size</code></td>
        
          <td><code>18px</code></td>
        
        <td><p>Size of the icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-show-focus-highlight</code></td>
        
          <td><code>false</code></td>
        
        <td><p>Show the focus highlight when the input has focus</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-show-valid-highlight</code></td>
        
          <td><code>$text-input-ios-show-focus-highlight</code></td>
        
        <td><p>Show the valid highlight when it is valid and has a value</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-show-invalid-highlight</code></td>
        
          <td><code>$text-input-ios-show-focus-highlight</code></td>
        
        <td><p>Show the invalid highlight when it is invalid and has value</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-highlight-color</code></td>
        
          <td><code>color($colors-ios, primary)</code></td>
        
        <td><p>Color of the input highlight</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-highlight-color-valid</code></td>
        
          <td><code>$text-input-highlight-color-valid</code></td>
        
        <td><p>Color of the input highlight when valid</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-ios-highlight-color-invalid</code></td>
        
          <td><code>$text-input-highlight-color-invalid</code></td>
        
        <td><p>Color of the input highlight when invalid</p>
</td>
      </tr>
      
    </tbody>
  </table>
  
  <table ng-show="active === 'md'" id="sass-md" class="table param-table" style="margin:0;">
    <thead>
      <tr>
        <th>Property</th>
        <th>Default</th>
        <th>Description</th>
      </tr>
    </thead>
    <tbody>
      
      <tr>
        <td><code>$text-input-md-background-color</code></td>
        
          <td><code>$list-md-background-color</code></td>
        
        <td><p>Background color of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-margin-top</code></td>
        
          <td><code>$item-md-padding-top</code></td>
        
        <td><p>Margin top of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-margin-right</code></td>
        
          <td><code>($item-md-padding-right / 2)</code></td>
        
        <td><p>Margin right of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-margin-bottom</code></td>
        
          <td><code>$item-md-padding-bottom</code></td>
        
        <td><p>Margin bottom of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-margin-left</code></td>
        
          <td><code>($item-md-padding-left / 2)</code></td>
        
        <td><p>Margin left of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-input-clear-icon-width</code></td>
        
          <td><code>30px</code></td>
        
        <td><p>Width of the icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-input-clear-icon-color</code></td>
        
          <td><code>#5b5b5b</code></td>
        
        <td><p>Color of the icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-input-clear-icon-svg</code></td>
        
          <td><code>&quot;&lt;svg xmlns=&#39;http://www.w3.org/2000/svg&#39; viewBox=&#39;0 0 512 512&#39;&gt;&lt;polygon fill=&#39;&quot; + $text-input-md-input-clear-icon-color + &quot;&#39; points=&#39;405,136.798 375.202,107 256,226.202 136.798,107 107,136.798 226.202,256 107,375.202 136.798,405 256,285.798 375.202,405 405,375.202 285.798,256&#39;/&gt;&lt;/svg&gt;&quot;</code></td>
        
        <td><p>Icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-input-clear-icon-size</code></td>
        
          <td><code>22px</code></td>
        
        <td><p>Size of the icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-show-focus-highlight</code></td>
        
          <td><code>true</code></td>
        
        <td><p>Show the focus highlight when the input has focus</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-show-valid-highlight</code></td>
        
          <td><code>$text-input-md-show-focus-highlight</code></td>
        
        <td><p>Show the valid highlight when it is valid and has a value</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-show-invalid-highlight</code></td>
        
          <td><code>$text-input-md-show-focus-highlight</code></td>
        
        <td><p>Show the invalid highlight when it is invalid and has value</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-highlight-color</code></td>
        
          <td><code>color($colors-md, primary)</code></td>
        
        <td><p>Color of the input highlight</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-highlight-color-valid</code></td>
        
          <td><code>$text-input-highlight-color-valid</code></td>
        
        <td><p>Color of the input highlight when valid</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-md-highlight-color-invalid</code></td>
        
          <td><code>$text-input-highlight-color-invalid</code></td>
        
        <td><p>Color of the input highlight when invalid</p>
</td>
      </tr>
      
    </tbody>
  </table>
  
  <table ng-show="active === 'wp'" id="sass-wp" class="table param-table" style="margin:0;">
    <thead>
      <tr>
        <th>Property</th>
        <th>Default</th>
        <th>Description</th>
      </tr>
    </thead>
    <tbody>
      
      <tr>
        <td><code>$text-input-wp-background-color</code></td>
        
          <td><code>$list-wp-background-color</code></td>
        
        <td><p>Background color of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-border-color</code></td>
        
          <td><code>$input-wp-border-color</code></td>
        
        <td><p>Border color of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-border-width</code></td>
        
          <td><code>2px</code></td>
        
        <td><p>Border width of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-margin-top</code></td>
        
          <td><code>$item-wp-padding-top</code></td>
        
        <td><p>Margin top of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-margin-right</code></td>
        
          <td><code>($item-wp-padding-right / 2)</code></td>
        
        <td><p>Margin right of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-margin-bottom</code></td>
        
          <td><code>$item-wp-padding-bottom</code></td>
        
        <td><p>Margin bottom of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-margin-left</code></td>
        
          <td><code>($item-wp-padding-left / 2)</code></td>
        
        <td><p>Margin left of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-padding-vertical</code></td>
        
          <td><code>0</code></td>
        
        <td><p>Vertical padding of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-padding-horizontal</code></td>
        
          <td><code>8px</code></td>
        
        <td><p>Horizontal padding of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-line-height</code></td>
        
          <td><code>3rem</code></td>
        
        <td><p>Line height of the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-input-clear-icon-width</code></td>
        
          <td><code>30px</code></td>
        
        <td><p>Width of the icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-input-clear-icon-color</code></td>
        
          <td><code>$input-wp-border-color</code></td>
        
        <td><p>Color of the icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-input-clear-icon-svg</code></td>
        
          <td><code>&quot;&lt;svg xmlns=&#39;http://www.w3.org/2000/svg&#39; viewBox=&#39;0 0 512 512&#39;&gt;&lt;polygon fill=&#39;&quot; + $text-input-wp-input-clear-icon-color + &quot;&#39; points=&#39;405,136.798 375.202,107 256,226.202 136.798,107 107,136.798 226.202,256 107,375.202 136.798,405 256,285.798 375.202,405 405,375.202 285.798,256&#39;/&gt;&lt;/svg&gt;&quot;</code></td>
        
        <td><p>Icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-input-clear-icon-size</code></td>
        
          <td><code>22px</code></td>
        
        <td><p>Size of the icon used to clear the input</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-show-focus-highlight</code></td>
        
          <td><code>true</code></td>
        
        <td><p>Show the focus highlight when the input has focus</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-show-valid-highlight</code></td>
        
          <td><code>$text-input-wp-show-focus-highlight</code></td>
        
        <td><p>Show the valid highlight when it is valid and has a value</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-show-invalid-highlight</code></td>
        
          <td><code>$text-input-wp-show-focus-highlight</code></td>
        
        <td><p>Show the invalid highlight when it is invalid and has value</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-highlight-color</code></td>
        
          <td><code>color($colors-wp, primary)</code></td>
        
        <td><p>Color of the input highlight</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-highlight-color-valid</code></td>
        
          <td><code>$text-input-highlight-color-valid</code></td>
        
        <td><p>Color of the input highlight when valid</p>
</td>
      </tr>
      
      <tr>
        <td><code>$text-input-wp-highlight-color-invalid</code></td>
        
          <td><code>$text-input-highlight-color-invalid</code></td>
        
        <td><p>Color of the input highlight when invalid</p>
</td>
      </tr>
      
    </tbody>
  </table>
  
</div>



<!-- related link --><!-- end content block -->


<!-- end body block -->

