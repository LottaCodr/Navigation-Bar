# Navigation-Bar
React Navigation Bar 
import React from 'react';
import "bootstrap/dist/css/bootstrap.min.css";
import { Navbar, Container, Form, Nav, Button, FormControl, NavDropdown } from "react-bootstrap";
import IMAGES from '../components/Images'




const Navigation = () => { 
    
    return (
           <Navbar collapseOnSelect bg="light" expand="lg" sticky="top">
                        
                            <Container>
                                <Navbar bg="light" variant="dark">
                                    <Container>
                                    <Navbar.Brand href="home">
                                        <img
                                            src={IMAGES.forweb}
                                            width="40"
                                            height="40"
                                            className="d-line-block align-top"
                                            alt="YTLogo"
                                            /> 
                                    </Navbar.Brand>
                                    </Container>
                                </Navbar>

                            <Navbar.Brand>
                                <Nav.Link > YelloTape Studio </Nav.Link>
                            </Navbar.Brand>
                            <Navbar.Toggle/>
                            <Navbar.Collapse id="responsive-navbar-nav" className="justify-content-end">
                        <Nav  className="me-auto" >
                                <Nav.Link  href="/home">Home</Nav.Link>                          
                                <Nav.Link   href="/Projects">Portfolio</Nav.Link>                           
                                <Nav.Link   href="/About">About</Nav.Link>                            
                                <NavDropdown  title="Services" id="basic-nav-dropdown">
                                <NavDropdown.Item href="#action/3.1">Visual Design</NavDropdown.Item>
                                <NavDropdown.Item href="#action/3.2">Logo Design & Branding </NavDropdown.Item>
                                <NavDropdown.Item href="#action/3.3">UI/UX Design</NavDropdown.Item>
                                <NavDropdown.Item href="#action/3.4">Web & Mobile App Development</NavDropdown.Item>
                                <NavDropdown.Item href="#action/3.5">Video illustration and Animation</NavDropdown.Item>
                                <NavDropdown.Item href="#action/3.5">Software Developer for Hire</NavDropdown.Item>
                                </NavDropdown>                           
                                <Nav.Link   href="/Contact-us">Contact Us</Nav.Link>                         
                        </Nav>
                        <Form className="d-flex">
                            <FormControl
                                type="search"
                                placeholder="Search"
                                className="me-2"
                                aria-label="Look"
                                />
                                <Button variant="outlines-success">Search</Button>
                        </Form>
                        </Navbar.Collapse>
                        </Container>
                        
            </Navbar>
    )
    
}
export default Navigation;
