# onsen

css styles to done
.btn {
    display: inline-block;
    padding: 0.9rem 1.8rem;
    font-size: 16px;
    font-weight: 700;
    color: white;
    border: 3px solid rgb(252, 70, 100);
    cursor: pointer;
    position: relative;
    background-color: transparent;
    text-decoration: none;
    overflow: hidden;
    z-index: 1;
    font-family: inherit;
}

.btn::before,
.btn::after {
    content: "";
    position: absolute;
    top: 0;
    height: 100%;
    background-color: rgb(252, 70, 100);
    transition: all .3s;
}

.btn::before {
    left: 50%;
    width: 0;
    transform: translateX(-50%);
}

.btn::after {
    right: 50%;
    width: 0;
    transform: translateX(50%);
}

.btn:hover::before {
    width: 100%;
}

.btn:hover::after {
    width: 100%;
}
