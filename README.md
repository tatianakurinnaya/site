App.js
import './App.css';
import {Route,BrowserRouter} from "react-router-dom";
import {Header} from "./components/Header";
import {Slider} from "./components/Slider";
import {About} from "./components/About";
import {Latestproducts} from "./components/Latestproducts";
import {Pricing} from "./components/Pricing";
import {Work} from "./components/Work";
import {Service} from "./components/Service";
import {Contact} from "./components/Contact";
import {Footer} from "./components/Footer";




function Menu() {
  return(
      <div className="menu">
        <a href="/">Главная</a> | <a href="/about">О нас</a> | <a href="/contact-us">Контакты</a>
      </div>
  )
}
function Content(){
  return <p>
    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus, consectetur dolor ea eos error hic illum incidunt iste itaque iusto mollitia nemo nihil nisi nobis nostrum officia perspiciatis, quam quia ratione suscipit totam ut velit veniam? Accusantium aliquid consectetur delectus esse eum fugit incidunt, magnam perferendis? Aperiam architecto atque consectetur consequatur, ducimus ex excepturi obcaecati?
  </p>
}


function App() {
  return (
      <div className="container">
          <BrowserRouter>
              <Header/>
              <Slider/>
              <About/>
              <Latestproducts/>
              <Pricing/>
              <Work/>
              <Service/>
              <Contact/>
              <Footer/>

              <Route exact path="/" component={()=><div>

              </div>}/>
              <Route path="/products" component={()=><div>
                  <p>Продукты</p>
              </div>}/>
              <Route path="/service" component={()=><div>
                  <p>Сервис</p>
              </div>}/>

          </BrowserRouter>
      </div>
  );
}

export default App;

Components:
About.jsx
import React from 'react'

export function About(){
    return(<div id="about">
        <div className="content-lg container">
            <div className="masonry-grid row">
                <div className="masonry-grid-sizer col-xs-6 col-sm-6 col-md-1"></div>
                <div className="masonry-grid-item col-xs-12 col-sm-6 col-md-4 sm-margin-b-30">
                    <div className="margin-b-60">
                        <h2>Art Of Coding</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incididunt ut laboret
                            dolore magna ut consequat siad esqudiat dolor</p>
                    </div>
                    <img className="full-width img-responsive wow fadeInUp" src="img/500x500/01.jpg"
                         alt="Portfolio Image" data-wow-duration=".3" data-wow-delay=".2s"/>
                </div>
                <div className="masonry-grid-item col-xs-12 col-sm-6 col-md-4">
                    <div className="margin-b-60">
                        <img className="full-width img-responsive wow fadeInUp" src="img/500x500/02.jpg"
                             alt="Portfolio Image" data-wow-duration=".3" data-wow-delay=".3s"/>
                    </div>
                    <h2>Clean Design</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incididunt ut laboret dolore
                        magna ut consequat siad esqudiat dolor</p>
                </div>
                <div className="masonry-grid-item col-xs-12 col-sm-6 col-md-4">
                    <div className="margin-t-60 margin-b-60">
                        <h2>Amazing Support</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incididunt ut laboret
                            dolore magna ut consequat siad esqudiat dolor</p>
                    </div>
                    <img className="full-width img-responsive wow fadeInUp" src="img/500x500/03.jpg"
                         alt="Portfolio Image" data-wow-duration=".3" data-wow-delay=".4s"/>
                </div>
            </div>
        </div>

        <div className="bg-color-sky-light">
            <div className="content-lg container">
                <div className="row">
                    <div className="col-md-5 col-sm-5 md-margin-b-60">
                        <div className="margin-t-50 margin-b-30">
                            <h2>Why Choose Us?</h2>
                            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
                                incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
                                exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
                        </div>
                        <a href="#" className="btn-theme btn-theme-sm btn-white-bg text-uppercase">Explore</a>
                    </div>
                    <div className="col-md-5 col-sm-7 col-md-offset-2">
                        <div className="accordion">
                            <div className="panel-group" id="accordion" role="tablist" aria-multiselectable="true">
                                <div className="panel panel-default">
                                    <div className="panel-heading" role="tab" id="headingOne">
                                        <h4 className="panel-title">
                                            <a className="panel-title-child" role="button" data-toggle="collapse"
                                               data-parent="#accordion" href="#collapseOne" aria-expanded="true"
                                               aria-controls="collapseOne">
                                                Exceptional Frontend Framework
                                            </a>
                                        </h4>
                                    </div>
                                    <div id="collapseOne" className="panel-collapse collapse in" role="tabpanel"
                                         aria-labelledby="headingOne">
                                        <div className="panel-body">
                                            Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                                            richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard
                                            dolor brunch.
                                        </div>
                                    </div>
                                </div>
                                <div className="panel panel-default">
                                    <div className="panel-heading" role="tab" id="headingTwo">
                                        <h4 className="panel-title">
                                            <a className="collapsed panel-title-child" role="button"
                                               data-toggle="collapse" data-parent="#accordion" href="#collapseTwo"
                                               aria-expanded="false" aria-controls="collapseTwo">
                                                Modern Design Trends
                                            </a>
                                        </h4>
                                    </div>
                                    <div id="collapseTwo" className="panel-collapse collapse" role="tabpanel"
                                         aria-labelledby="headingTwo">
                                        <div className="panel-body">
                                            Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                                            richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard
                                            dolor brunch.
                                        </div>
                                    </div>
                                </div>
                                <div className="panel panel-default">
                                    <div className="panel-heading" role="tab" id="headingThree">
                                        <h4 className="panel-title">
                                            <a className="collapsed panel-title-child" role="button"
                                               data-toggle="collapse" data-parent="#accordion" href="#collapseThree"
                                               aria-expanded="false" aria-controls="collapseThree">
                                                Beatifully Crafted Code
                                            </a>
                                        </h4>
                                    </div>
                                    <div id="collapseThree" className="panel-collapse collapse" role="tabpanel"
                                         aria-labelledby="headingThree">
                                        <div className="panel-body">
                                            Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                                            richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard
                                            dolor brunch.
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>)
}

Contact.jsx
import React from "react"

export function Contact(){
    return(<div id="contact">
        <div className="section-seperator">
            <div className="content-lg container">
                <div className="row">
                    <div className="col-sm-4 sm-margin-b-50">
                        <h3><a href="#">New York</a> <span className="text-uppercase margin-l-20">Head Office</span>
                        </h3>
                        <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incdidunt ut laboret dolor
                            magna ut consequat siad esqudiat dolor</p>
                        <ul className="list-unstyled contact-list">
                            <li><i className="margin-r-10 color-base icon-call-out"></i> 1 012 3456 7890</li>
                            <li><i className="margin-r-10 color-base icon-envelope"></i> hq@aitOnepage.com</li>
                        </ul>
                    </div>

                    <div className="col-sm-4 sm-margin-b-50">
                        <h3><a href="#">London</a> <span className="text-uppercase margin-l-20">Operation</span></h3>
                        <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incdidunt ut laboret dolor
                            magna ut consequat siad esqudiat dolor</p>
                        <ul className="list-unstyled contact-list">
                            <li><i className="margin-r-10 color-base icon-call-out"></i> 44 77 3456 7890</li>
                            <li><i className="margin-r-10 color-base icon-envelope"></i> operation@AitOnepage.com</li>
                        </ul>
                    </div>

                    <div className="col-sm-4 sm-margin-b-50">
                        <h3><a href="#">Singapore</a> <span className="text-uppercase margin-l-20">Finance</span></h3>
                        <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incdidunt ut laboret dolor
                            magna ut consequat siad esqudiat dolor</p>
                        <ul className="list-unstyled contact-list">
                            <li><i className="margin-r-10 color-base icon-call-out"></i> 50 012 456 7890</li>
                            <li><i className="margin-r-10 color-base icon-envelope"></i> finance@AitOnepage.com</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div id="map" className="map height-300"></div>
    </div>)
}

Footer.jsx
import React from 'react'

export function Footer(){
    return(<footer className="footer">
        <div className="section-seperator">
            <div className="content-md container">
                <div className="row">
                    <div className="col-sm-2 sm-margin-b-30">
                        <ul className="list-unstyled footer-list">
                            <li className="footer-list-item"><a href="#">Home</a></li>
                            <li className="footer-list-item"><a href="#">About</a></li>
                            <li className="footer-list-item"><a href="#">Work</a></li>
                            <li className="footer-list-item"><a href="#">Contact</a></li>
                        </ul>
                    </div>
                    <div className="col-sm-2 sm-margin-b-30">
                        <ul className="list-unstyled footer-list">
                            <li className="footer-list-item"><a href="#">Twitter</a></li>
                            <li className="footer-list-item"><a href="#">Facebook</a></li>
                            <li className="footer-list-item"><a href="#">Instagram</a></li>
                            <li className="footer-list-item"><a href="#">YouTube</a></li>
                        </ul>
                    </div>
                    <div className="col-sm-3">
                        <ul className="list-unstyled footer-list">
                            <li className="footer-list-item"><a href="#">Subscribe to Our Newsletter</a></li>
                            <li className="footer-list-item"><a href="#">Privacy Policy</a></li>
                            <li className="footer-list-item"><a href="#">Terms &amp; Conditions</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div className="content container">
            <div className="row">
                <div className="col-xs-6">
                    <img className="footer-logo" src="img/logo-dark.png" alt="Aitonepage Logo"/>
                </div>
                <div className="col-xs-6 text-right">
                    <p className="margin-b-0"><a className="fweight-700"
                                                 href="http://keenthemes.com/preview/aitonepage/">Aitonepage</a> Theme
                        Powered by: <a className="fweight-700" href="http://www.keenthemes.com/">KeenThemes.com</a></p>
                </div>
            </div>
        </div>
    </footer>)
}

Header.jsx
import React from 'react'

export function Header(){
    return(<header className="header navbar-fixed-top">
        <nav className="navbar" role="navigation">
            <div className="container">
                <div className="menu-container js_nav-item">
                    <button type="button" className="navbar-toggle" data-toggle="collapse" data-target=".nav-collapse">
                        <span className="sr-only">Toggle navigation</span>
                        <span className="toggle-icon"></span>
                    </button>

                    <div className="logo">
                        <a className="logo-wrap" href="#body">
                            <img className="logo-img logo-img-main" src="img/logo.png" alt="Asentus Logo"/>
                                <img className="logo-img logo-img-active" src="img/logo-dark.png" alt="Asentus Logo"/>
                        </a>
                    </div>
                </div>

                <div className="collapse navbar-collapse nav-collapse">
                    <div className="menu-container">
                        <ul className="nav navbar-nav navbar-nav-right">
                            <li className="js_nav-item nav-item"><a className="nav-item-child nav-item-hover"
                                                                    href="#body">Home</a></li>
                            <li className="js_nav-item nav-item"><a className="nav-item-child nav-item-hover"
                                                                    href="#about">About</a></li>
                            <li className="js_nav-item nav-item"><a className="nav-item-child nav-item-hover"
                                                                    href="#products">Products</a></li>
                            <li className="js_nav-item nav-item"><a className="nav-item-child nav-item-hover"
                                                                    href="#pricing">Pricing</a></li>
                            <li className="js_nav-item nav-item"><a className="nav-item-child nav-item-hover"
                                                                    href="#work">Work</a></li>
                            <li className="js_nav-item nav-item"><a className="nav-item-child nav-item-hover"
                                                                    href="#service">Service</a></li>
                            <li className="js_nav-item nav-item"><a className="nav-item-child nav-item-hover"
                                                                    href="#contact">Contact</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </nav>
    </header>)
}

Latestproducts.jsx
import React from 'react'

export function Latestproducts(){
    return(<div id="products">
        <div className="content-lg container">
            <div className="row margin-b-40">
                <div className="col-sm-6">
                    <h2>Latest Products</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incididunt ut laboret dolore
                        magna aliqua enim minim veniam exercitation</p>
                </div>
            </div>


            <div className="row">

                <div className="col-sm-4 sm-margin-b-50">
                    <div className="margin-b-20">
                        <img className="img-responsive" src="img/970x647/01.jpg" alt="Latest Products Image"/>
                    </div>
                    <h4><a href="#">Workspace</a> <span className="text-uppercase margin-l-20">Management</span></h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incdidunt ut laboret dolor
                        magna ut consequat siad esqudiat dolor</p>
                    <a className="link" href="#">Read More</a>
                </div>

                <div className="col-sm-4 sm-margin-b-50">
                    <div className="margin-b-20">
                        <img className="img-responsive" src="img/970x647/02.jpg" alt="Latest Products Image"/>
                    </div>
                    <h4><a href="#">Minimalism</a> <span className="text-uppercase margin-l-20">Developmeny</span></h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incdidunt ut laboret dolor
                        magna ut consequat siad esqudiat dolor</p>
                    <a className="link" href="#">Read More</a>
                </div>

                <div className="col-sm-4 sm-margin-b-50">
                    <div className="margin-b-20">
                        <img className="img-responsive" src="img/970x647/03.jpg" alt="Latest Products Image"/>
                    </div>
                    <h4><a href="#">Cleant Style</a> <span className="text-uppercase margin-l-20">Design</span></h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incdidunt ut laboret dolor
                        magna ut consequat siad esqudiat dolor</p>
                    <a className="link" href="#">Read More</a>
                </div>
            </div>
        </div>
    </div>)
}

Pricing.jsx
import React from 'react'

export function Pricing(){
    return(<div id="pricing">
        <div className="bg-color-sky-light">
            <div className="content-lg container">
                <div className="row row-space-1">
                    <div className="col-sm-4 sm-margin-b-2">
                        <div className="pricing">
                            <div className="margin-b-30">
                                <i className="pricing-icon icon-chemistry"></i>
                                <h3>Starter Kit <span> - $</span> 49</h3>
                                <p>Lorem ipsum dolor amet consectetur ut consequat siad esqudiat dolor</p>
                            </div>
                            <ul className="list-unstyled pricing-list margin-b-50">
                                <li className="pricing-list-item">Basic Features</li>
                                <li className="pricing-list-item">Up to 5 products</li>
                                <li className="pricing-list-item">50 Users Panels</li>
                            </ul>
                            <a href="pricing.html"
                               className="btn-theme btn-theme-sm btn-default-bg text-uppercase">Choose</a>
                        </div>
                    </div>
                    <div className="col-sm-4 sm-margin-b-2">
                        <div className="pricing pricing-active">
                            <div className="margin-b-30">
                                <i className="pricing-icon icon-badge"></i>
                                <h3>Professional <span> - $</span> 149</h3>
                                <p>Lorem ipsum dolor amet consectetur ut consequat siad esqudiat dolor</p>
                            </div>
                            <ul className="list-unstyled pricing-list margin-b-50">
                                <li className="pricing-list-item">Basic Features</li>
                                <li className="pricing-list-item">Up to 100 products</li>
                                <li className="pricing-list-item">100 Users Panels</li>
                            </ul>
                            <a href="pricing.html"
                               className="btn-theme btn-theme-sm btn-default-bg text-uppercase">Choose</a>
                        </div>
                    </div>
                    <div className="col-sm-4">
                        <div className="pricing">
                            <div className="margin-b-30">
                                <i className="pricing-icon icon-shield"></i>
                                <h3>Advanced <span> - $</span> 249</h3>
                                <p>Lorem ipsum dolor amet consectetur ut consequat siad esqudiat dolor</p>
                            </div>
                            <ul className="list-unstyled pricing-list margin-b-50">
                                <li className="pricing-list-item">Extended Features</li>
                                <li className="pricing-list-item">Unlimited products</li>
                                <li className="pricing-list-item">Unlimited Users Panels</li>
                            </ul>
                            <a href="pricing.html"
                               className="btn-theme btn-theme-sm btn-default-bg text-uppercase">Choose</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>)
}

Service.jsx 
import React from 'react'

export function Service(){
    return(<div id="service">
        <div className="bg-color-sky-light" data-auto-height="true">
            <div className="content-lg container">
                <div className="row margin-b-40">
                    <div className="col-sm-6">
                        <h2>Services</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incididunt ut laboret
                            dolore magna aliqua enim minim veniam exercitation</p>
                    </div>
                </div>

                <div className="row row-space-1 margin-b-2">
                    <div className="col-sm-4 sm-margin-b-2">
                        <div className="service" data-height="height">
                            <div className="service-element">
                                <i className="service-icon icon-chemistry"></i>
                            </div>
                            <div className="service-info">
                                <h3>Art Of Coding</h3>
                                <p className="margin-b-5">Lorem ipsum dolor amet consectetur ut consequat siad esqudiat
                                    dolor</p>
                            </div>
                            <a href="#" className="content-wrapper-link"></a>
                        </div>
                    </div>
                    <div className="col-sm-4 sm-margin-b-2">
                        <div className="service bg-color-base" data-height="height">
                            <div className="service-element">
                                <i className="service-icon color-white icon-screen-tablet"></i>
                            </div>
                            <div className="service-info">
                                <h3 className="color-white">Responsive Design</h3>
                                <p className="color-white margin-b-5">Lorem ipsum dolor amet consectetur ut consequat
                                    siad esqudiat dolor</p>
                            </div>
                            <a href="#" className="content-wrapper-link"></a>
                        </div>
                    </div>
                    <div className="col-sm-4">
                        <div className="service" data-height="height">
                            <div className="service-element">
                                <i className="service-icon icon-badge"></i>
                            </div>
                            <div className="service-info">
                                <h3>Feature Reach</h3>
                                <p className="margin-b-5">Lorem ipsum dolor amet consectetur ut consequat siad esqudiat
                                    dolor</p>
                            </div>
                            <a href="#" className="content-wrapper-link"></a>
                        </div>
                    </div>
                </div>

                <div className="row row-space-1">
                    <div className="col-sm-4 sm-margin-b-2">
                        <div className="service" data-height="height">
                            <div className="service-element">
                                <i className="service-icon icon-notebook"></i>
                            </div>
                            <div className="service-info">
                                <h3>Useful Documentation</h3>
                                <p className="margin-b-5">Lorem ipsum dolor amet consectetur ut consequat siad esqudiat
                                    dolor</p>
                            </div>
                            <a href="#" className="content-wrapper-link"></a>
                        </div>
                    </div>
                    <div className="col-sm-4 sm-margin-b-2">
                        <div className="service" data-height="height">
                            <div className="service-element">
                                <i className="service-icon icon-speedometer"></i>
                            </div>
                            <div className="service-info">
                                <h3>Fast Delivery</h3>
                                <p className="margin-b-5">Lorem ipsum dolor amet consectetur ut consequat siad esqudiat
                                    dolor</p>
                            </div>
                            <a href="#" className="content-wrapper-link"></a>
                        </div>
                    </div>
                    <div className="col-sm-4">
                        <div className="service" data-height="height">
                            <div className="service-element">
                                <i className="service-icon icon-badge"></i>
                            </div>
                            <div className="service-info">
                                <h3>Free Plugins</h3>
                                <p className="margin-b-5">Lorem ipsum dolor amet consectetur ut consequat siad esqudiat
                                    dolor</p>
                            </div>
                            <a href="#" className="content-wrapper-link"></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>)
}

Slider.jsx
 import React from 'react'

 export function Slider(){
    return(<div id="carousel-example-generic" className="carousel slide" data-ride="carousel">
        <div className="container">
            <ol className="carousel-indicators">
                <li data-target="#carousel-example-generic" data-slide-to="0" className="active"></li>
                <li data-target="#carousel-example-generic" data-slide-to="1"></li>
            </ol>
        </div>

        <div className="carousel-inner" role="listbox">
            <div className="item active">
                <img className="img-responsive" src="img/1920x1080/01.jpg" alt="Slider Image"/>
                    <div className="container">
                        <div className="carousel-centered">
                            <div className="margin-b-40">
                                <h1 className="carousel-title">Hi-Tech Design</h1>
                                <p className="color-white">Lorem ipsum dolor amet consectetur adipiscing dolore magna
                                    aliqua <br/> enim minim estudiat veniam siad venumus dolore</p>
                            </div>
                            <a href="#" className="btn-theme btn-theme-sm btn-white-brd text-uppercase">Explore</a>
                        </div>
                    </div>
            </div>
            <div className="item">
                <img className="img-responsive" src="img/1920x1080/02.jpg" alt="Slider Image"/>
                    <div className="container">
                        <div className="carousel-centered">
                            <div className="margin-b-40">
                                <h2 className="carousel-title">Hi-Tech Design</h2>
                                <p className="color-white">Lorem ipsum dolor amet consectetur adipiscing dolore magna
                                    aliqua <br/> enim minim estudiat veniam siad venumus dolore</p>
                            </div>
                            <a href="#" className="btn-theme btn-theme-sm btn-white-brd text-uppercase">Explore</a>
                        </div>
                    </div>
            </div>
        </div>
    </div>)
 }
 
 Work.jsx
 import React from 'react'

export function Work(){
    return(<div id="work">
        <div className="section-seperator">
            <div className="content-md container">
                <div className="row margin-b-40">
                    <div className="col-sm-6">
                        <h2>Work</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipiscing elit sed tempor incididunt ut laboret
                            dolore magna aliqua enim minim veniam exercitation</p>
                    </div>
                </div>

                <div className="masonry-grid row">
                    <div className="masonry-grid-sizer col-xs-6 col-sm-6 col-md-1"></div>
                    <div className="masonry-grid-item col-xs-12 col-sm-6 col-md-8 margin-b-30">
                        <div className="work work-popup-trigger">
                            <div className="work-overlay">
                                <img className="full-width img-responsive" src="img/800x400/01.jpg"
                                     alt="Portfolio Image"/>
                            </div>
                            <div className="work-popup-overlay">
                                <div className="work-popup-content">
                                    <a href="javascript:void(0);" className="work-popup-close">Hide</a>
                                    <div className="margin-b-30">
                                        <h3 className="margin-b-5">Art Of Coding</h3>
                                        <span>Clean &amp; Minimalistic Design</span>
                                    </div>
                                    <div className="row">
                                        <div className="col-sm-8 work-popup-content-divider sm-margin-b-20">
                                            <div className="margin-t-10 sm-margin-t-0">
                                                <p>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
                                                    dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
                                                    non proident, sunt in culpa qui officia deserunt mollit anim id est
                                                    laborum.</p>
                                                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
                                                    eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
                                                    ad minim veniam, quis nostrud.</p>
                                                <ul className="list-inline work-popup-tag">
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Design,</a></li>
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Coding,</a></li>
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Portfolio</a></li>
                                                </ul>
                                            </div>
                                        </div>
                                        <div className="col-sm-4">
                                            <div className="margin-t-10 sm-margin-t-0">
                                                <p className="margin-b-5"><strong>Project Leader:</strong> John Doe</p>
                                                <p className="margin-b-5"><strong>Designer:</strong> Alisa Keys</p>
                                                <p className="margin-b-5"><strong>Developer:</strong> Mark Doe</p>
                                                <p className="margin-b-5"><strong>Customer:</strong> Keenthemes</p>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div className="masonry-grid-item col-xs-12 col-sm-6 col-md-4 margin-b-30">
                        <div className="work work-popup-trigger">
                            <div className="work-overlay">
                                <img className="full-width img-responsive" src="img/397x415/01.jpg"
                                     alt="Portfolio Image"/>
                            </div>
                            <div className="work-popup-overlay">
                                <div className="work-popup-content">
                                    <a href="javascript:void(0);" className="work-popup-close">Hide</a>
                                    <div className="margin-b-30">
                                        <h3 className="margin-b-5">Art Of Coding</h3>
                                        <span>Clean &amp; Minimalistic Design</span>
                                    </div>
                                    <div className="row">
                                        <div className="col-sm-8 work-popup-content-divider sm-margin-b-20">
                                            <div className="margin-t-10 sm-margin-t-0">
                                                <p>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
                                                    dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
                                                    non proident, sunt in culpa qui officia deserunt mollit anim id est
                                                    laborum.</p>
                                                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
                                                    eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
                                                    ad minim veniam, quis nostrud.</p>
                                                <ul className="list-inline work-popup-tag">
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Design,</a></li>
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Coding,</a></li>
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Portfolio</a></li>
                                                </ul>
                                            </div>
                                        </div>
                                        <div className="col-sm-4">
                                            <div className="margin-t-10 sm-margin-t-0">
                                                <p className="margin-b-5"><strong>Project Leader:</strong> John Doe</p>
                                                <p className="margin-b-5"><strong>Designer:</strong> Alisa Keys</p>
                                                <p className="margin-b-5"><strong>Developer:</strong> Mark Doe</p>
                                                <p className="margin-b-5"><strong>Customer:</strong> Keenthemes</p>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div className="masonry-grid-item col-xs-12 col-sm-6 col-md-4 md-margin-b-30">
                        <div className="work work-popup-trigger">
                            <div className="work-overlay">
                                <img className="full-width img-responsive" src="img/397x300/01.jpg"
                                     alt="Portfolio Image"/>
                            </div>
                            <div className="work-popup-overlay">
                                <div className="work-popup-content">
                                    <a href="javascript:void(0);" className="work-popup-close">Hide</a>
                                    <div className="margin-b-30">
                                        <h3 className="margin-b-5">Art Of Coding</h3>
                                        <span>Clean &amp; Minimalistic Design</span>
                                    </div>
                                    <div className="row">
                                        <div className="col-sm-8 work-popup-content-divider sm-margin-b-20">
                                            <div className="margin-t-10 sm-margin-t-0">
                                                <p>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
                                                    dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
                                                    non proident, sunt in culpa qui officia deserunt mollit anim id est
                                                    laborum.</p>
                                                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
                                                    eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
                                                    ad minim veniam, quis nostrud.</p>
                                                <ul className="list-inline work-popup-tag">
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Design,</a></li>
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Coding,</a></li>
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Portfolio</a></li>
                                                </ul>
                                            </div>
                                        </div>
                                        <div className="col-sm-4">
                                            <div className="margin-t-10 sm-margin-t-0">
                                                <p className="margin-b-5"><strong>Project Leader:</strong> John Doe</p>
                                                <p className="margin-b-5"><strong>Designer:</strong> Alisa Keys</p>
                                                <p className="margin-b-5"><strong>Developer:</strong> Mark Doe</p>
                                                <p className="margin-b-5"><strong>Customer:</strong> Keenthemes</p>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div className="masonry-grid-item col-xs-12 col-sm-6 col-md-4 md-margin-b-30">
                        <div className="work work-popup-trigger">
                            <div className="work-overlay">
                                <img className="full-width img-responsive" src="img/397x300/02.jpg"
                                     alt="Portfolio Image"/>
                            </div>
                            <div className="work-popup-overlay">
                                <div className="work-popup-content">
                                    <a href="javascript:void(0);" className="work-popup-close">Hide</a>
                                    <div className="margin-b-30">
                                        <h3 className="margin-b-5">Art Of Coding</h3>
                                        <span>Clean &amp; Minimalistic Design</span>
                                    </div>
                                    <div className="row">
                                        <div className="col-sm-8 work-popup-content-divider sm-margin-b-20">
                                            <div className="margin-t-10 sm-margin-t-0">
                                                <p>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
                                                    dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
                                                    non proident, sunt in culpa qui officia deserunt mollit anim id est
                                                    laborum.</p>
                                                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
                                                    eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
                                                    ad minim veniam, quis nostrud.</p>
                                                <ul className="list-inline work-popup-tag">
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Design,</a></li>
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Coding,</a></li>
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Portfolio</a></li>
                                                </ul>
                                            </div>
                                        </div>
                                        <div className="col-sm-4">
                                            <div className="margin-t-10 sm-margin-t-0">
                                                <p className="margin-b-5"><strong>Project Leader:</strong> John Doe</p>
                                                <p className="margin-b-5"><strong>Designer:</strong> Alisa Keys</p>
                                                <p className="margin-b-5"><strong>Developer:</strong> Mark Doe</p>
                                                <p className="margin-b-5"><strong>Customer:</strong> Keenthemes</p>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div className="masonry-grid-item col-xs-12 col-sm-6 col-md-4">
                        <div className="work work-popup-trigger">
                            <div className="work-overlay">
                                <img className="full-width img-responsive" src="img/397x300/03.jpg"
                                     alt="Portfolio Image"/>
                            </div>
                            <div className="work-popup-overlay">
                                <div className="work-popup-content">
                                    <a href="javascript:void(0);" className="work-popup-close">Hide</a>
                                    <div className="margin-b-30">
                                        <h3 className="margin-b-5">Art Of Coding</h3>
                                        <span>Clean &amp; Minimalistic Design</span>
                                    </div>
                                    <div className="row">
                                        <div className="col-sm-8 work-popup-content-divider sm-margin-b-20">
                                            <div className="margin-t-10 sm-margin-t-0">
                                                <p>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
                                                    dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
                                                    non proident, sunt in culpa qui officia deserunt mollit anim id est
                                                    laborum.</p>
                                                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
                                                    eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
                                                    ad minim veniam, quis nostrud.</p>
                                                <ul className="list-inline work-popup-tag">
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Design,</a></li>
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Coding,</a></li>
                                                    <li className="work-popup-tag-item"><a
                                                        className="work-popup-tag-link" href="#">Portfolio</a></li>
                                                </ul>
                                            </div>
                                        </div>
                                        <div className="col-sm-4">
                                            <div className="margin-t-10 sm-margin-t-0">
                                                <p className="margin-b-5"><strong>Project Leader:</strong> John Doe</p>
                                                <p className="margin-b-5"><strong>Designer:</strong> Alisa Keys</p>
                                                <p className="margin-b-5"><strong>Developer:</strong> Mark Doe</p>
                                                <p className="margin-b-5"><strong>Customer:</strong> Keenthemes</p>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div className="content-lg container">
            <div className="swiper-slider swiper-clients">
                <div className="swiper-wrapper">
                    <div className="swiper-slide">
                        <img className="swiper-clients-img" src="img/clients/01.png" alt="Clients Logo"/>
                    </div>
                    <div className="swiper-slide">
                        <img className="swiper-clients-img" src="img/clients/02.png" alt="Clients Logo"/>
                    </div>
                    <div className="swiper-slide">
                        <img className="swiper-clients-img" src="img/clients/03.png" alt="Clients Logo"/>
                    </div>
                    <div className="swiper-slide">
                        <img className="swiper-clients-img" src="img/clients/04.png" alt="Clients Logo"/>
                    </div>
                    <div className="swiper-slide">
                        <img className="swiper-clients-img" src="img/clients/05.png" alt="Clients Logo"/>
                    </div>
                    <div className="swiper-slide">
                        <img className="swiper-clients-img" src="img/clients/06.png" alt="Clients Logo"/>
                    </div>
                </div>
            </div>
        </div>
    </div>)
}
