# TextFiled-
TextFiled 键盘处理
- (void)configKeyBoardRespond {
    self.keyboardUtil = [[ZYKeyboardUtil alloc] init];
    
    __weak LoginVC *weakSelf = self;
    
    //全自动键盘弹出处理
    [_keyboardUtil setAnimateWhenKeyboardAppearAutomaticAnimBlock:^(ZYKeyboardUtil *keyboardUtil) {
        [keyboardUtil adaptiveViewHandleWithController:weakSelf adaptiveView:weakSelf.text所在view, weakSelf.text1,weakSelf.text1, weakSelf.text3, nil];
    }];
    
}
